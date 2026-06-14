# OpenWeatherMap GraphQL Schema

This is a conceptual GraphQL schema for the OpenWeatherMap API surface. OpenWeatherMap does not publish a native GraphQL endpoint; this schema is a structured representation of the REST API resources available at [openweathermap.org/api](https://openweathermap.org/api) and serves as a reference for building GraphQL wrappers, federated gateway layers, or code-generation targets.

## Coverage

The schema covers all major OpenWeatherMap product areas:

| Area | Types |
|---|---|
| Current Weather | `Weather`, `CurrentWeather`, `WeatherCondition`, `WeatherGroup`, `WeatherDescription` |
| Forecasts | `MinuteForecast`, `HourlyForecast`, `DailyForecast`, `Forecast5Day`, `Forecast16Day` |
| Atmospheric Parameters | `Temperature`, `Pressure`, `Humidity`, `Clouds`, `Visibility` |
| Wind | `Wind`, `WindSpeed`, `WindGust`, `WindDegree` |
| Precipitation | `Rain`, `Snow`, `Precipitation` |
| Celestial | `Sunrise`, `Sunset`, `MoonPhase`, `Tide` |
| UV | `UVIndex` |
| Air Quality | `AirQuality`, `AirComponents`, `AirPollution`, `AirQualityMain`, `AirPollutionList` |
| Alerts | `WeatherAlert`, `Alerts`, `AlertMetadata` |
| Geocoding | `Coordinates`, `Geocode`, `GeocodeResult`, `ReverseGeocode` |
| Location | `City`, `Country` |
| History | `WeatherHistory`, `WeatherArchive`, `WeatherStat` |
| Solar | `SolarIrradiance`, `SolarPanelOutput` |
| Maps | `WeatherMap`, `TileLayer` |
| Stations | `Station`, `StationData` |
| API / Account | `WeatherAPI`, `APICall`, `APIQuota`, `APISubscription` |

## Type Count

The schema defines **55 named types** (object types, enums, and scalars), plus `Query` and `Mutation` root types.

## Enums

- `TemperatureUnit` — KELVIN, CELSIUS, FAHRENHEIT
- `WindSpeedUnit` — METERS_PER_SECOND, MILES_PER_HOUR, KILOMETERS_PER_HOUR, KNOTS
- `AQILevel` — GOOD, FAIR, MODERATE, POOR, VERY_POOR
- `WeatherMapLayer` — CLOUDS, PRECIPITATION, SEA_LEVEL_PRESSURE, WIND_SPEED, TEMPERATURE, HUMIDITY
- `ForecastInterval` — HOURLY, THREE_HOURLY, DAILY, MINUTE
- `StationGranularity` — MINUTE, HOUR, DAY
- `PollutantType` — CO, NO, NO2, O3, SO2, NH3, PM2_5, PM10
- `SolarComponent` — GHI, DNI, DHI

## Query Examples

### Current weather by city name

```graphql
query {
  currentWeatherByCity(city: "London", countryCode: "GB", units: CELSIUS) {
    dt
    temp
    feelsLike
    humidity { value }
    pressure { value }
    wind {
      speed { value unit }
      deg { value cardinal }
    }
    conditions {
      main
      description
      icon
    }
    sunrise { dt }
    sunset { dt }
  }
}
```

### One Call — full weather timeline

```graphql
query {
  oneCall(lat: 51.5074, lon: -0.1278, units: CELSIUS) {
    current {
      temp
      uvIndex { value risk }
      clouds { all }
      rain { oneHour }
    }
    hourly {
      dt
      temp
      pop
      wind { speed { value } deg { value } }
    }
    daily {
      dt
      temp { min max }
      conditions { description }
      moonPhase { value name }
    }
    alerts {
      event
      start
      end
      description
    }
  }
}
```

### Air pollution forecast

```graphql
query {
  airPollutionForecast(lat: 48.8566, lon: 2.3522) {
    list {
      dt
      main { aqi }
      components {
        pm2_5
        pm10
        no2
        o3
      }
    }
  }
}
```

### Forward geocoding

```graphql
query {
  geocode(q: "Paris,FR", limit: 5) {
    query
    results {
      name
      lat
      lon
      country
      state
    }
  }
}
```

### Register a weather station (mutation)

```graphql
mutation {
  createStation(
    externalId: "MY_ROOF_01"
    name: "Roof Sensor"
    latitude: 51.5074
    longitude: -0.1278
    altitude: 42.0
  ) {
    id
    name
    rank
  }
}
```

## Mapping to REST Endpoints

| GraphQL Query / Mutation | REST Equivalent |
|---|---|
| `currentWeatherByCity` | `GET /data/2.5/weather?q={city}` |
| `currentWeatherByCoords` | `GET /data/2.5/weather?lat={lat}&lon={lon}` |
| `forecast5DayByCity` | `GET /data/2.5/forecast?q={city}` |
| `forecast16Day` | `GET /data/2.5/forecast/daily` |
| `oneCall` | `GET /data/4.0/onecall` |
| `oneCallHistory` | `GET /data/4.0/onecall/timemachine` |
| `airPollutionCurrent` | `GET /data/2.5/air_pollution` |
| `airPollutionForecast` | `GET /data/2.5/air_pollution/forecast` |
| `airPollutionHistory` | `GET /data/2.5/air_pollution/history` |
| `geocode` | `GET /geo/1.0/direct` |
| `geocodeByZip` | `GET /geo/1.0/zip` |
| `reverseGeocode` | `GET /geo/1.0/reverse` |
| `weatherHistory` | `GET /data/2.5/history/city` |
| `weatherStats` | `GET /data/2.5/aggregated/day` |
| `solarIrradiance` | `GET /energy/2.0/solar/irradiance` |
| `stations` | `GET /data/3.0/stations` |
| `createStation` | `POST /data/3.0/stations` |
| `deleteStation` | `DELETE /data/3.0/stations/{id}` |

## Authentication

All queries require an OpenWeatherMap API key passed as the `appid` query parameter in the underlying REST calls. In a GraphQL gateway implementation this would typically be forwarded via an HTTP header:

```
Authorization: Bearer <API_KEY>
```

or as a custom header:

```
X-OWM-API-Key: <API_KEY>
```

## References

- API Catalog: https://openweathermap.org/api
- One Call 4.0: https://openweathermap.org/api/one-call-4
- Air Pollution API: https://openweathermap.org/api/air-pollution
- Geocoding API: https://openweathermap.org/api/geocoding-api
- GitHub Organization: https://github.com/OpenWeatherMap
- Weather Stations: https://openweathermap.org/stations
- Solar Irradiance: https://openweathermap.org/api/solar-irradiance
- Weather Maps: https://openweathermap.org/api/weathermaps

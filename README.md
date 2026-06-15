# OpenWeatherMap (openweathermap)

OpenWeather (operating openweathermap.org) is a global weather data platform delivering current weather, multi-horizon forecasts, historical archives, climate statistics, air pollution, solar irradiance, road risk, geocoding, and weather map tiles. Data is sourced from satellites, weather models, radars, and a worldwide network of weather stations, served through REST APIs across a freemium, multi-tier, and pay-per-call commercial model.

**APIs.json:** [https://openweathermap.org/api](https://openweathermap.org/api)

## Tags

- Weather
- Forecast
- Climate
- Air Pollution
- Air Quality
- Solar
- Geocoding
- History
- Maps
- Road Risk
- Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## APIs

### Current Weather Data API

Returns current weather data for any location on Earth, including over 200,000 cities, sourced from satellites, radars, models, and a global network of weather stations.

- **Human URL:** [https://openweathermap.org/current](https://openweathermap.org/current)
- **Base URL:** `https://api.openweathermap.org/data/2.5`

#### Tags

- Weather
- Current Weather

#### Properties

- [Documentation](https://openweathermap.org/current)
- [OpenAPI](openapi/openweathermap-current-weather-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openweathermap-current-weather.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openweathermap-current-weather.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/openweathermap-current-weather-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/openweathermap-current-weather-structure.json)
- [Example](examples/current-weather-example.json)
- [Authentication](https://openweathermap.org/appid)

### Forecast APIs

OpenWeather forecast surface including the public 5-day/3-hour forecast plus pro hourly (4 days), daily (16 days), and climatic (30 days) forecasts.

- **Human URL:** [https://openweathermap.org/forecast5](https://openweathermap.org/forecast5)
- **Base URL:** `https://api.openweathermap.org/data/2.5`

#### Tags

- Weather
- Forecast

#### Properties

- [Documentation](https://openweathermap.org/forecast5)
- [Documentation](https://openweathermap.org/api/hourly-forecast)
- [Documentation](https://openweathermap.org/forecast16)
- [Documentation](https://openweathermap.org/api/forecast30)
- [OpenAPI](openapi/openweathermap-forecast-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openweathermap-forecast.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openweathermap-forecast.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/openweathermap-forecast-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/forecast-five-day-example.json)

### One Call API 4.0

Unified weather timeline including current conditions, hourly, daily, 1-minute precipitation, 15-minute forecasts, government weather alerts, and 47 plus years of historical data via pay-per-call pricing.

- **Human URL:** [https://openweathermap.org/api/one-call-4](https://openweathermap.org/api/one-call-4)
- **Base URL:** `https://api.openweathermap.org/data/4.0/onecall`

#### Tags

- Weather
- Forecast
- History

#### Properties

- [Documentation](https://openweathermap.org/api/one-call-4)
- [OpenAPI](openapi/openweathermap-one-call-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openweathermap-one-call.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openweathermap-one-call.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/one-call-current-example.json)

### Air Pollution API

Current, forecast, and historical air pollution data including the Air Quality Index and concentrations of CO, NO, NO2, O3, SO2, NH3, PM2.5, and PM10 for any coordinates on the globe.

- **Human URL:** [https://openweathermap.org/api/air-pollution](https://openweathermap.org/api/air-pollution)
- **Base URL:** `https://api.openweathermap.org/data/2.5`

#### Tags

- Air Pollution
- Air Quality

#### Properties

- [Documentation](https://openweathermap.org/api/air-pollution)
- [OpenAPI](openapi/openweathermap-air-pollution-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openweathermap-air-pollution.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openweathermap-air-pollution.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/openweathermap-air-pollution-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/openweathermap-air-pollution-structure.json)
- [Example](examples/air-pollution-current-example.json)

### Geocoding API

Direct and reverse geocoding for city names, postal codes, and coordinate pairs. Supports city, state, country, and area-level resolution.

- **Human URL:** [https://openweathermap.org/api/geocoding-api](https://openweathermap.org/api/geocoding-api)
- **Base URL:** `https://api.openweathermap.org/geo/1.0`

#### Tags

- Geocoding

#### Properties

- [Documentation](https://openweathermap.org/api/geocoding-api)
- [OpenAPI](openapi/openweathermap-geocoding-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openweathermap-geocoding.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openweathermap-geocoding.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/openweathermap-geocoding-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/openweathermap-geocoding-structure.json)
- [Example](examples/geocoding-direct-example.json)

### Historical Weather API

Historical weather observations for any global coordinate at one-hour granularity, spanning 47 plus years. Available on Professional and Expert plans.

- **Human URL:** [https://openweathermap.org/history](https://openweathermap.org/history)
- **Base URL:** `https://history.openweathermap.org/data/2.5`

#### Tags

- Weather
- History

#### Properties

- [Documentation](https://openweathermap.org/history)
- [OpenAPI](openapi/openweathermap-history-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openweathermap-history.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openweathermap-history.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/history-city-example.json)

### Statistical Weather Data API

Statistical aggregates (record min/max, average, mean, percentiles, standard deviation) for main weather parameters on any day, month, or yearly basis. Expert plan only.

- **Human URL:** [https://openweathermap.org/api/statistics-api](https://openweathermap.org/api/statistics-api)
- **Base URL:** `https://history.openweathermap.org/data/2.5`

#### Tags

- Weather
- Climate
- Statistics

#### Properties

- [Documentation](https://openweathermap.org/api/statistics-api)
- [OpenAPI](openapi/openweathermap-statistical-weather-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openweathermap-statistical-weather.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openweathermap-statistical-weather.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/statistical-month-example.json)

### Accumulated Parameters API

Accumulated temperature and precipitation totals over a historical time window, primarily for agriculture and energy applications. Available on Professional and Expert plans.

- **Human URL:** [https://openweathermap.org/api/accumulated-parameters](https://openweathermap.org/api/accumulated-parameters)
- **Base URL:** `https://history.openweathermap.org/data/2.5/history`

#### Tags

- Weather
- History
- Agriculture

#### Properties

- [Documentation](https://openweathermap.org/api/accumulated-parameters)
- [OpenAPI](openapi/openweathermap-accumulated-parameters-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openweathermap-accumulated-parameters.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openweathermap-accumulated-parameters.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/accumulated-temperature-example.json)

### Solar Energy APIs

Solar Irradiance API (GHI, DNI, DHI for clear and cloudy sky models, 15 minute or hourly intervals, 47 plus years history) and Solar Panel Energy Prediction API (manage modeled locations and solar panel configurations and retrieve per-panel power and energy output).

- **Human URL:** [https://openweathermap.org/api/solar-irradiance](https://openweathermap.org/api/solar-irradiance)
- **Base URL:** `https://api.openweathermap.org/energy/2.0`

#### Tags

- Solar
- Energy

#### Properties

- [Documentation](https://openweathermap.org/api/solar-irradiance)
- [Documentation](https://openweathermap.org/api/solar-panels-and-energy-prediction-2)
- [OpenAPI](openapi/openweathermap-solar-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openweathermap-solar.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openweathermap-solar.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/solar-irradiance-interval-example.json)

### Road Risk API

Route-specific weather data, national alerts, current conditions plus five-day forecast, and one year of historical data for a sequence of waypoints. Custom quote required.

- **Human URL:** [https://openweathermap.org/api/road-risk](https://openweathermap.org/api/road-risk)
- **Base URL:** `https://api.openweathermap.org`

#### Tags

- Weather
- Routing
- Risk

#### Properties

- [Documentation](https://openweathermap.org/api/road-risk)
- [OpenAPI](openapi/openweathermap-road-risk-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openweathermap-road-risk.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openweathermap-road-risk.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/road-risk-example.json)

### Weather Stations API

Register and manage personal weather stations and submit measurement data. Aggregated readings are retrievable at minute, hour, and day granularity.

- **Human URL:** [https://openweathermap.org/stations](https://openweathermap.org/stations)
- **Base URL:** `https://api.openweathermap.org/data/3.0`

#### Tags

- Weather
- Stations
- IoT

#### Properties

- [Documentation](https://openweathermap.org/stations)
- [OpenAPI](openapi/openweathermap-weather-stations-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openweathermap-weather-stations.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openweathermap-weather-stations.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/openweathermap-station-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/weather-stations-create-example.json)

### Weather Maps 1.0

Tile map service overlaying weather data layers (clouds, precipitation, pressure, wind, temperature) on top of base maps using standard z/x/y tile coordinates. Compatible with Leaflet, OpenLayers, Google Maps.

- **Human URL:** [https://openweathermap.org/api/weathermaps](https://openweathermap.org/api/weathermaps)
- **Base URL:** `https://tile.openweathermap.org`

#### Tags

- Weather
- Maps
- Tiles

#### Properties

- [Documentation](https://openweathermap.org/api/weathermaps)
- [OpenAPI](openapi/openweathermap-weather-maps-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/openweathermap-weather-maps.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/openweathermap-weather-maps.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/weather-maps-tile-example.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Website](https://openweathermap.org/)
- [Developer Portal](https://openweathermap.org/api)
- [Getting Started](https://openweathermap.org/guide)
- [API Reference](https://openweathermap.org/api)
- [Authentication](https://openweathermap.org/appid)
- [Sign Up](https://home.openweathermap.org/users/sign_up)
- [Login](https://home.openweathermap.org/users/sign_in)
- [Console](https://dashboard.openweather.co.uk/)
- [Pricing](https://openweathermap.org/price)
- [Plans](plans/openweathermap-plans-pricing.yml)
- [Rate Limits](rate-limits/openweathermap-rate-limits.yml)
- [Marketplace](https://openweathermap.org/marketplace)
- [Blog](https://openweather.co.uk/blog)
- [F A Q](https://openweathermap.org/faq)
- [Support](https://openweathermap.org/support-centre)
- [Terms of Service](https://openweather.co.uk/terms)
- [Privacy Policy](https://openweather.co.uk/privacy-policy)
- [GitHub Organization](https://github.com/OpenWeatherMap)
- [LinkedIn](https://www.linkedin.com/company/openweathermap)
- [Spectral Rules](rules/openweathermap-rules.yml)
- [Vocabulary](vocabulary/openweathermap-vocabulary.yml)
- [JSON-LD](json-ld/openweathermap-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)
- [Kubernetes C R D](undefined)
- [Tools](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com

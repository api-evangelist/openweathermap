# OpenWeatherMap (openweathermap)

OpenWeather (operating openweathermap.org) is a global weather data platform delivering current weather, multi-horizon forecasts, historical archives, climate statistics, air pollution, solar irradiance, road risk, geocoding, and weather map tiles. Data is sourced from satellites, weather models, radars, and a worldwide network of weather stations, served through REST APIs across a freemium, multi-tier, and pay-per-call commercial model.

**URL:** [https://openweathermap.org/api](https://openweathermap.org/api)

## Scope

- **Type:** Company
- **Category:** Weather
- **Tier:** 2 — comprehensive weather suite with multi-tier pricing

## Tags

Weather, Forecast, Climate, Air Pollution, Air Quality, Solar, Geocoding, History, Maps, Road Risk

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## APIs

### Current Weather Data API
Returns current weather data for any location on Earth, including over 200,000 cities, sourced from satellites, radars, models, and a global network of weather stations.

- Human URL: https://openweathermap.org/current
- Base URL: https://api.openweathermap.org/data/2.5
- OpenAPI: [openapi/openweathermap-current-weather-openapi.yml](openapi/openweathermap-current-weather-openapi.yml)
- JSON Schema: [json-schema/openweathermap-current-weather-schema.json](json-schema/openweathermap-current-weather-schema.json)
- JSON Structure: [json-structure/openweathermap-current-weather-structure.json](json-structure/openweathermap-current-weather-structure.json)
- Capability: [capabilities/current-weather.yaml](capabilities/current-weather.yaml)
- Example: [examples/current-weather-example.json](examples/current-weather-example.json)

### Forecast APIs
OpenWeather forecast surface including the public 5-day/3-hour forecast plus pro hourly (4 days), daily (16 days), and climatic (30 days) forecasts.

- Human URL: https://openweathermap.org/forecast5
- OpenAPI: [openapi/openweathermap-forecast-openapi.yml](openapi/openweathermap-forecast-openapi.yml)
- JSON Schema: [json-schema/openweathermap-forecast-schema.json](json-schema/openweathermap-forecast-schema.json)
- Capability: [capabilities/forecast.yaml](capabilities/forecast.yaml)
- Example: [examples/forecast-five-day-example.json](examples/forecast-five-day-example.json)

### One Call API 4.0
Unified weather timeline including current conditions, hourly, daily, 1-minute precipitation, 15-minute forecasts, government weather alerts, and 47+ years of historical data via pay-per-call pricing.

- Human URL: https://openweathermap.org/api/one-call-4
- Base URL: https://api.openweathermap.org/data/4.0/onecall
- OpenAPI: [openapi/openweathermap-one-call-openapi.yml](openapi/openweathermap-one-call-openapi.yml)
- Capability: [capabilities/one-call.yaml](capabilities/one-call.yaml)
- Example: [examples/one-call-current-example.json](examples/one-call-current-example.json)

### Air Pollution API
Current, forecast, and historical air pollution data including the Air Quality Index and concentrations of CO, NO, NO2, O3, SO2, NH3, PM2.5, and PM10 for any coordinates on the globe.

- Human URL: https://openweathermap.org/api/air-pollution
- OpenAPI: [openapi/openweathermap-air-pollution-openapi.yml](openapi/openweathermap-air-pollution-openapi.yml)
- JSON Schema: [json-schema/openweathermap-air-pollution-schema.json](json-schema/openweathermap-air-pollution-schema.json)
- JSON Structure: [json-structure/openweathermap-air-pollution-structure.json](json-structure/openweathermap-air-pollution-structure.json)
- Capability: [capabilities/air-pollution.yaml](capabilities/air-pollution.yaml)
- Example: [examples/air-pollution-current-example.json](examples/air-pollution-current-example.json)

### Geocoding API
Direct and reverse geocoding for city names, postal codes, and coordinate pairs. Supports city, state, country, and area-level resolution.

- Human URL: https://openweathermap.org/api/geocoding-api
- OpenAPI: [openapi/openweathermap-geocoding-openapi.yml](openapi/openweathermap-geocoding-openapi.yml)
- JSON Schema: [json-schema/openweathermap-geocoding-schema.json](json-schema/openweathermap-geocoding-schema.json)
- JSON Structure: [json-structure/openweathermap-geocoding-structure.json](json-structure/openweathermap-geocoding-structure.json)
- Capability: [capabilities/geocoding.yaml](capabilities/geocoding.yaml)
- Example: [examples/geocoding-direct-example.json](examples/geocoding-direct-example.json)

### Historical Weather API
Historical weather observations for any global coordinate at one-hour granularity, spanning 47+ years. Available on Professional and Expert plans.

- Human URL: https://openweathermap.org/history
- OpenAPI: [openapi/openweathermap-history-openapi.yml](openapi/openweathermap-history-openapi.yml)
- Capability: [capabilities/history.yaml](capabilities/history.yaml)
- Example: [examples/history-city-example.json](examples/history-city-example.json)

### Statistical Weather Data API
Statistical aggregates (record min/max, average, mean, percentiles, standard deviation) for main weather parameters on any day, month, or yearly basis. Expert plan only.

- Human URL: https://openweathermap.org/api/statistics-api
- OpenAPI: [openapi/openweathermap-statistical-weather-openapi.yml](openapi/openweathermap-statistical-weather-openapi.yml)
- Example: [examples/statistical-month-example.json](examples/statistical-month-example.json)

### Accumulated Parameters API
Accumulated temperature and precipitation totals over a historical time window, primarily for agriculture and energy applications. Available on Professional and Expert plans.

- Human URL: https://openweathermap.org/api/accumulated-parameters
- OpenAPI: [openapi/openweathermap-accumulated-parameters-openapi.yml](openapi/openweathermap-accumulated-parameters-openapi.yml)
- Example: [examples/accumulated-temperature-example.json](examples/accumulated-temperature-example.json)

### Solar Energy APIs
Solar Irradiance API (GHI, DNI, DHI for clear and cloudy sky models, 15-minute or hourly intervals, 47+ years history) and Solar Panel Energy Prediction API (manage modeled locations and solar panel configurations, retrieve per-panel power and energy output).

- Human URL: https://openweathermap.org/api/solar-irradiance
- OpenAPI: [openapi/openweathermap-solar-openapi.yml](openapi/openweathermap-solar-openapi.yml)
- Capability: [capabilities/solar.yaml](capabilities/solar.yaml)
- Example: [examples/solar-irradiance-interval-example.json](examples/solar-irradiance-interval-example.json)

### Road Risk API
Route-specific weather data, national alerts, current conditions plus five-day forecast, and one year of historical data for a sequence of waypoints. Custom quote required.

- Human URL: https://openweathermap.org/api/road-risk
- OpenAPI: [openapi/openweathermap-road-risk-openapi.yml](openapi/openweathermap-road-risk-openapi.yml)
- Example: [examples/road-risk-example.json](examples/road-risk-example.json)

### Weather Stations API
Register and manage personal weather stations and submit measurement data. Aggregated readings are retrievable at minute, hour, and day granularity.

- Human URL: https://openweathermap.org/stations
- OpenAPI: [openapi/openweathermap-weather-stations-openapi.yml](openapi/openweathermap-weather-stations-openapi.yml)
- JSON Schema: [json-schema/openweathermap-station-schema.json](json-schema/openweathermap-station-schema.json)
- Example: [examples/weather-stations-create-example.json](examples/weather-stations-create-example.json)

### Weather Maps 1.0
Tile map service overlaying weather data layers (clouds, precipitation, pressure, wind, temperature) on top of base maps using standard z/x/y tile coordinates. Compatible with Leaflet, OpenLayers, and Google Maps.

- Human URL: https://openweathermap.org/api/weathermaps
- OpenAPI: [openapi/openweathermap-weather-maps-openapi.yml](openapi/openweathermap-weather-maps-openapi.yml)
- Example: [examples/weather-maps-tile-example.json](examples/weather-maps-tile-example.json)

## Plans, Rate Limits, and FinOps

- Plans and Pricing: [plans/openweathermap-plans-pricing.yml](plans/openweathermap-plans-pricing.yml)
- Rate Limits: [rate-limits/openweathermap-rate-limits.yml](rate-limits/openweathermap-rate-limits.yml)
- FinOps: [finops/openweathermap-finops.yml](finops/openweathermap-finops.yml)

OpenWeather operates a tiered subscription model (Free, Startup, Developer, Professional, Expert) plus a One Call 4.0 pay-per-call plan (first 1,000 daily calls free) and custom enterprise contracts. Per-tier rate ceilings range from 60 calls/minute on Free to 100,000 calls/minute on Expert, with monthly quotas from 1M up to 3B requests. See the rate-limits artifact for the full per-API breakdown.

## Cross-Cutting Artifacts

- Spectral rules: [rules/openweathermap-rules.yml](rules/openweathermap-rules.yml)
- Vocabulary: [vocabulary/openweathermap-vocabulary.yml](vocabulary/openweathermap-vocabulary.yml)
- JSON-LD context: [json-ld/openweathermap-context.jsonld](json-ld/openweathermap-context.jsonld)

## Tools and Ecosystem

OpenWeather has a vibrant MCP and skills ecosystem:

- MCP servers: NimbleBrainInc/mcp-openweathermap, robertn702/mcp-openweathermap, fgladisch/openweathermap-mcp-server, jezweb/weather-mcp-server, SaintDoresh/Weather-MCP-ClaudeDesktop, tristau/openweathermap-mcp
- Claude Code skills: kevinl95/ForecastSkill, OpenWeather API Automation (MCPmarket)
- OpenWeather-published OSS: VANE geospatial platform, Deker storage engine, leaflet-weather-layer, leaflet-coupled-layers, weatherchecker-go, awesome-openweather

## Common Properties

- Website: https://openweathermap.org/
- Developer Portal: https://openweathermap.org/api
- Getting Started: https://openweathermap.org/guide
- API Reference: https://openweathermap.org/api
- Sign Up: https://home.openweathermap.org/users/sign_up
- Console: https://dashboard.openweather.co.uk/
- Pricing: https://openweathermap.org/price
- Marketplace: https://openweathermap.org/marketplace
- Blog: https://openweather.co.uk/blog
- FAQ: https://openweathermap.org/faq
- Support: https://openweathermap.org/support-centre
- Terms of Service: https://openweather.co.uk/terms
- Privacy Policy: https://openweather.co.uk/privacy-policy
- GitHub: https://github.com/OpenWeatherMap
- LinkedIn: https://www.linkedin.com/company/openweathermap

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com

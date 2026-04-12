# immichframe-stack

Docker Compose stack for **immichframe-stack**.

## Services

| Service | Image |
|---------|-------|
| immichframe | `ghcr.io/immichframe/immichframe:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `Albums` — see compose for default
- `ApiKey` — replace with actual value
- `AuthenticationSecret` — replace with actual value
- `ClockFormat` — see compose for default
- `DownloadImages` — see compose for default
- `ImageLocationFormat` — see compose for default
- `ImagePan` — see compose for default
- `ImageZoom` — see compose for default
- `ImmichServerUrl` — see compose for default
- `Interval` — see compose for default
- `Language` — see compose for default
- `Layout` — see compose for default
- `PLAYBACK_MODE` — see compose for default
- `PhotoDateFormat` — see compose for default
- `RenewImagesDuration` — see compose for default
- `ShowClock` — see compose for default
- `ShowImageLocation` — see compose for default
- `ShowPeopleDesc` — see compose for default
- `ShowPhotoDate` — see compose for default
- `ShowVideos` — see compose for default
- `ShowWeatherDescription` — see compose for default
- `TZ` — see compose for default
- `TransitionDuration` — see compose for default
- `UnitSystem` — see compose for default
- `WeatherApiKey` — replace with actual value
- `WeatherLatLong` — see compose for default

## Volumes

- /path/to/your/data

## Networks

default

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout

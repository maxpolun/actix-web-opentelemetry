# Changelog

## [v0.11.0-beta.2](https://github.com/OutThereLabs/actix-web-opentelemetry/compare/v0.11.0-beta.1..v0.11.0-beta.2)

### Changed

- Update to actix-web `4.0.0-beta.4` and awc `3.0.0-beta.3` (#57)

## [v0.11.0-beta.1](https://github.com/OutThereLabs/actix-web-opentelemetry/compare/v0.10.0...v0.11.0-beta.1)

### Changed

- Update to tokio `1.0` and actix-web `4.0.0-beta.3` (#51)

## [v0.10.0](https://github.com/OutThereLabs/actix-web-opentelemetry/compare/v0.9.0...v0.10.0)

### Changed

Note: optentelemetry `v0.12.x` uses tokio 1.0. See the
[updated examples](https://github.com/OutThereLabs/actix-web-opentelemetry/blob/e29c77312d6a906571286f78cc26ca72cf3a0b6f/examples/server.rs#L17-L40)
for compatible setup until actix-web supports tokio 1.0.

- Update to OpenTelemetry v0.12.x #48

## [v0.9.0](https://github.com/OutThereLabs/actix-web-opentelemetry/compare/v0.8.0...v0.9.0)

### Changed

- Update to OpenTelemetry v0.11.x #41

## [v0.8.0](https://github.com/OutThereLabs/actix-web-opentelemetry/compare/v0.7.0...v0.8.0)

Be sure to set a trace propagator via [`global::set_text_map_propagator`](https://docs.rs/opentelemetry/0.10.0/opentelemetry/global/fn.set_text_map_propagator.html)
as the default is now a no-op.

### Changed

- Update to OpenTelemetry v0.10.x #38

## [v0.7.0](https://github.com/OutThereLabs/actix-web-opentelemetry/compare/v0.6.0...v0.7.0)

### Changed

- Remove default features from actix-web #30
- Update to OpenTelemetry v0.9.x #30
- Move metrics behind a feature flag #30
- Change default route name from unmatched to default #30

### Removed

- Remove deprecated `with_tracing` function. #30

## [v0.6.0](https://github.com/OutThereLabs/actix-web-opentelemetry/compare/v0.5.0...v0.6.0)

### Changed

- Upgrade `actix-web` to version 3 #24
- `RequestMetrics` constructor longer accept a route_formatter. Can be added via `with_route_formatter` #24

### Removed

- Remove obsolute `UuidWildcardFormatter` as actix 3 supports match patterns #24

### Fixed

- Client will now properly inject context using the globally configured
  propagator.

## [v0.5.0](https://github.com/OutThereLabs/actix-web-opentelemetry/compare/v0.4.0...v0.5.0)

### Added

- Trace actix client requests with `ClientExt::trace_request` or
  `ClientExt::trace_request_with_context`. #17

### Changed

- Update to OpenTelemetry v0.8.0 #18
- Deprecated `with_tracing` fn. Use `ClientExt` instead. #17

## [v0.4.0](https://github.com/OutThereLabs/actix-web-opentelemetry/compare/v0.3.0...v0.4.0)

### Changed

- Update to OpenTelemetry v0.7.0 #11

## [v0.3.0](https://github.com/OutThereLabs/actix-web-opentelemetry/compare/v0.2.0...v0.3.0)

### Changed

- Update to OpenTelemetry v0.6.0 #10

## [v0.2.0](https://github.com/OutThereLabs/actix-web-opentelemetry/compare/v0.1.2...v0.2.0)

### Changed

- Update to OpenTelemetry v0.2.0 #6

## [v0.1.2](https://github.com/OutThereLabs/actix-web-opentelemetry/compare/v0.1.1...v0.1.2)

### Changed

- Make client span name match otel spec #3

## [v0.1.1](https://github.com/OutThereLabs/actix-web-opentelemetry/compare/v0.1.0...v0.1.1)

### Added

- Add option for route formatter #1
- Add metrics middleware #2

## [v0.1.0](https://github.com/OutThereLabs/actix-web-opentelemetry/tree/v0.1.0)

Initial debug alpha

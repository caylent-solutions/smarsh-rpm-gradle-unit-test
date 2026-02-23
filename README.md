# smarsh-rpm-gradle-unit-test

RPM package providing TestNG framework configuration, JaCoCo code coverage, and a dedicated unitTest task.

## Provided Tasks

- `test` - Run unit tests (excludes integration tests)
- `unitTest` - Run unit tests only (alias with same exclusions)
- `jacocoTestReport` - Generate coverage report (HTML, XML, CSV)

## Configuration

- Test framework: TestNG
- JaCoCo tool version: 0.8.8
- Test logging: PASSED, SKIPPED, FAILED events
- Integration test exclusion: `**/integration/**`
- Coverage reports: XML, CSV, HTML

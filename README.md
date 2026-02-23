# smarsh-rpm-gradle-unit-test

RPM package providing TestNG framework configuration, JaCoCo code coverage, and a dedicated unitTest task.

## What This Package Does

Applies the JaCoCo Gradle plugin for code coverage and configures TestNG as the test framework. The standard `test` task is configured to exclude integration tests (anything in `**/integration/**`), and a dedicated `unitTest` alias task is provided. Coverage reports are generated automatically after tests run.

## Tasks Provided

| Task | Description |
|---|---|
| `test` | Run unit tests (excludes integration tests) |
| `unitTest` | Run unit tests only (alias with same exclusions) |
| `jacocoTestReport` | Generate coverage report (HTML, XML, CSV) |

## Configs and Assets

| File | Purpose | Synced To |
|---|---|---|
| `unit-test.gradle` | TestNG configuration, JaCoCo plugin setup, test exclusions, coverage reporting | `.packages/smarsh-rpm-gradle-unit-test/` |

## Configuration

- Test framework: TestNG
- JaCoCo tool version: 0.8.8
- Test logging: PASSED, SKIPPED, FAILED events
- Integration test exclusion: `**/integration/**`
- Coverage reports: XML, CSV, HTML

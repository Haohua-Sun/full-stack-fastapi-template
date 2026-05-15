# FastAPI Application Under Test

[简体中文](README.md) | English

[![API Automation Tests](https://github.com/Haohua-Sun/full-stack-fastapi-template/actions/workflows/api-automation-tests.yml/badge.svg)](https://github.com/Haohua-Sun/full-stack-fastapi-template/actions/workflows/api-automation-tests.yml)

This repository is forked from [`fastapi/full-stack-fastapi-template`](https://github.com/fastapi/full-stack-fastapi-template). In my API automation project, it is used as the application under test.

Related test repository:

```text
https://github.com/Haohua-Sun/fastapi-pytest-api-tests
```

## Repository Relationship

- `full-stack-fastapi-template`: provides the FastAPI backend, PostgreSQL database, OpenAPI contract, and business APIs.
- `fastapi-pytest-api-tests`: validates this repository's API behavior with `pytest`, `requests`, Allure, and database assertions.

When the test repository changes, its CI checks out and starts this application before running API tests. When this repository changes, [.github/workflows/api-automation-tests.yml](.github/workflows/api-automation-tests.yml) checks out the test repository and runs API regression tests against the current application version.

## Original Project

This fork keeps the main structure of the original FastAPI full-stack template. For framework details, local development, deployment, backend, and frontend documentation, refer to the upstream repository:

```text
https://github.com/fastapi/full-stack-fastapi-template
```

## License

The original Full Stack FastAPI Template is licensed under the MIT license.

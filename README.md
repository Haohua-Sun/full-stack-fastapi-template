# FastAPI 被测应用仓库

简体中文 | [English](README.en.md)

[![API Automation Tests](https://github.com/Haohua-Sun/full-stack-fastapi-template/actions/workflows/api-automation-tests.yml/badge.svg)](https://github.com/Haohua-Sun/full-stack-fastapi-template/actions/workflows/api-automation-tests.yml)

本仓库 fork 自 [`fastapi/full-stack-fastapi-template`](https://github.com/fastapi/full-stack-fastapi-template)，在我的接口自动化测试项目中作为被测应用使用。

对应测试仓库：[fastapi-pytest-api-tests](https://github.com/Haohua-Sun/fastapi-pytest-api-tests)

## 仓库关系

- `full-stack-fastapi-template`：提供 FastAPI backend、PostgreSQL、OpenAPI 契约和业务接口。
- `fastapi-pytest-api-tests`：使用 `pytest`、`requests`、Allure 和数据库断言验证本仓库的 API 行为。

测试仓库 push 时，会拉取并启动本仓库执行 API 测试。本仓库 push 时，也会通过 [.github/workflows/api-automation-tests.yml](.github/workflows/api-automation-tests.yml) 拉取测试仓库并执行 API 回归测试。

## 原项目参考

本仓库保留原 FastAPI 全栈模板的主要结构。框架说明、本地开发、部署和前后端细节请参考原仓库：[fastapi/full-stack-fastapi-template](https://github.com/fastapi/full-stack-fastapi-template)。

## License

The original Full Stack FastAPI Template is licensed under the MIT license.

# Stirling-PDF for TOS 7 (Docker)

本地运行的 PDF 工具箱：合并、拆分、压缩、格式转换、OCR、加密与水印等五十多种操作，文件只在 NAS 上处理，不上传到外部服务。

A locally hosted PDF toolbox with more than fifty operations such as merge, split, compress, convert, OCR, encryption and watermarking; files are processed on the NAS only.

## Package

- Application ID: `stirling-pdf`
- Type: Docker (TOS 7)
- Architecture: `x86_64`, `aarch64`
- Upstream image: see `docker-compose.yml` in the downloaded asset
- Web UI port: declared in `x-app-meta`

## Install

1. In the TOS App Center, add this repository's application and submit the matching `stirling-pdf_<arch>.tar.gz` asset from the latest Release.
2. Data is stored under `/Volume<N>/DockerAppData/stirling-pdf/` through the compose bind mounts.

## Notes

默认不启用登录认证；如需访问控制，请在应用配置中把 SECURITY_ENABLELOGIN 改为 true。配置、日志与临时文件保存在应用数据目录。

This repository packages the upstream open-source application for TerraMaster TOS 7.
It is not affiliated with or endorsed by the upstream project. Application names and
trademarks belong to their respective owners. All images are pulled from Docker Hub.

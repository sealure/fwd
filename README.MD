# Docker 部署指南

## 前置条件
- 系统已安装 Docker

## 使用 Docker 运行

拉取并运行镜像：

```bash
docker pull ghcr.io/sealure/fwd:latest
docker run -d --name fwd -p 7860:7860 --restart always ghcr.io/sealure/fwd:latest
```

## 使用 Docker Compose 运行

1. 进入 `compose` 目录：
```bash
cd compose
```

2. 启动服务：
```bash
docker compose up -d
```

3. 停止服务：
```bash
docker compose down
```

## 配置

环境变量：
- `DEFAULT_UUID`: 应用 UUID（默认值：f693501c-f468-442c-bcd2-6d7e118c8d41）

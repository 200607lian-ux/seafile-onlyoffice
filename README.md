# Seafile + OnlyOffice + Nginx 部署配置

## 项目结构
- `seafile/` - Seafile 服务配置
- `Docker-DocumentServer/` - OnlyOffice 文档服务配置  
- `nginx/` - Nginx 反向代理配置

## 核心配置文件
- `seafile/seafile-server.yml` - Seafile 主服务编排
- `seafile/caddy.yml` - Caddy 配置
- `seafile/seadoc.yml` - SeaDoc 文档服务
- `seafile/.env.example` - 环境变量模板
- `Docker-DocumentServer/docker-compose.yml` - OnlyOffice 编排
- `nginx/docker-compose.yml` - Nginx 编排
- `nginx/conf/nginx.conf` - Nginx 主配置
- `nginx/conf/seafile.conf` - Seafile 站点配置
- `nginx/conf/default.conf` - Nginx 默认配置

## 使用说明
1. 复制 `seafile/.env.example` 为 `seafile/.env`
2. 修改环境变量中的密码和配置
3. 按顺序启动服务

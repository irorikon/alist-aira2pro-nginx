## alist + aira2 的 Docker 实现方案

### 1. 安装 Docker

前往 [Docker-CE Install](https://docs.docker.com/engine/install/)

### 2. 部署

* 创建 nginx-config 文件夹

  ```bash
  mkdir -p nginx-config/ssl
  ```
* 编辑 nginx conf 文件

  ```bash
  vi nginx-config/alist.conf
  ```
* 开启 SSL（可选）

  * 在 nginx config 文件中指定证书位置，并将文件链接进 Docker 即可
  * 创建 docker-compose.yml 文件
  * 根据个人配置修改 docker-compose.yml 内容，保存即可
* 运行

  ```bash
  docker compose up -d
  ```

### 3. 访问

浏览器访问配置的网址 [example.com](example.com)

默认 Aira2 RPC 地址: example.com 443 jsonrpc

默认 Aria2 RPC 密钥: alist

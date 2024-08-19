# Inspect 部署指南

1. 复制配置文件至`config`

   ```bash
   $ mkdir config
   $ cp config.example.js config/config.js
   ```

2. 根据需要调整配置文件，主要是调整：

   1. logins

      Steam账号

   2. max_simultaneous_requests

      同一个IP的并发数，在局域网情况下可设置为-1

   3. bulk_key

      使用批量接口时的token

3. 启动服务

   ```bash
   $ docker compose up -d
   $ tail -10f config/index.log	# 查看输出日志
   ```

   
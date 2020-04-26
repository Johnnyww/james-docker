
前台运行并查看日志：
docker run
-p 25:25
-p 143:143
-p 110:110
--name james
chenjunxin/james-docker:v3.3.0

后台启动：
docker run -d
-p 25:25
-p 143:143
-p 110:110
--name james
chenjunxin/james-docker:v3.3.0

查看 后台启动时 最后10条日志(并实时跟踪新日志)：
docker logs -tf --tail 10 james

进入 后台启动时 容器：
docker exec -it james /bin/bash

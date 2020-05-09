# 视频播放上传网站
### 前端
基于vue和element-ui构建，进入front-end 使用npm run dev运行  
前端运行在8000端口上

### 后台
基于spring MVC构建，mvn jib:dockerBuild可以生成docker镜像，通过docker运行加haproxy均衡负载可以实现水平扩展，也可以通过mvn spring-boot:run运行在单个服务器上
后台端口为8080,haproxy默认使用4个端口均衡负载，为8081,8082,8083,8084  
视频分辨率压制使用了ffmpeg
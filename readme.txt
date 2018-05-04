#环境配置  maven build版本 3.3.9 插件版本 3.5.3



java -jar  xxx.jar --spring.profiles.active=peer1#启用哪个

#关于打包生成docker镜像
mvnw install #由于在pom文件中配置了执行任务所以在执行install时会走dockerfile：build，如果需要后面再执行push则可以添加<goal>push</goal>

#启动docker镜像，并起一个容器名
\cartoon_eurekaServer\cartoon_eurekaServer>docker run --name="eureka-server"  -p 8081:8081 -t zhangshexin/scp/e
urekaserver





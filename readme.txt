java -jar  xxx.jar --spring.profiles.active=peer1#启用哪个

#关于打包生成docker镜像
mvnw install #由于在pom文件中配置了执行任务所以在执行install时会走dockerfile：build，如果需要后面再执行push则可以添加<goal>push</goal>
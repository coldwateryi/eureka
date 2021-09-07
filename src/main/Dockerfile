FROM 10.211.55.9/system_containers/java:8

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

RUN mkdir -p /eureka

WORKDIR /eureka

EXPOSE 8761

ADD /shared/eureka/demo-0.0.1-SNAPSHOT.jar ./

CMD java -Djava.security.egd=file:/dev/./urandom -jar demo-0.0.1-SNAPSHOT.jar

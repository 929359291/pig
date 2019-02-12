FROM fabric8/java-alpine-openjdk8-jre

MAINTAINER wangiegie@gmail.com

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

RUN mkdir -p /pig-upms

WORKDIR /pig-upms

EXPOSE 4000

ADD ./pig-upms/pig-upms-biz/target/pig-upms-biz.jar ./

CMD java -Djava.security.egd=file:/dev/./urandom -jar pig-upms-biz.jar

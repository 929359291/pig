FROM fabric8/java-alpine-openjdk8-jre

MAINTAINER wangiegie@gmail.com

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

RUN mkdir -p /pig-codegen

WORKDIR /pig-codegen

EXPOSE 5003

ADD ./pig-visual/pig-codegen/target/pig-codegen.jar ./

CMD java -Djava.security.egd=file:/dev/./urandom -jar pig-codegen.jar

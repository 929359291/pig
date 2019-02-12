FROM fabric8/java-alpine-openjdk8-jre

MAINTAINER wangiegie@gmail.com

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

RUN mkdir -p /pig-auth

WORKDIR /pig-auth

EXPOSE 3000

ADD ./pig-auth/target/pig-auth.jar ./

CMD java -Djava.security.egd=file:/dev/./urandom -jar pig-auth.jar

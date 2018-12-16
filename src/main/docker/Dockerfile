FROM openjdk:11.0.1-jdk-oracle


ADD target/config-*.jar app.jar
ADD src/main/docker/entrypoint.sh entrypoint.sh
RUN chmod +x entrypoint.sh

ENV SERVER_GIT_URI=""
ENV SERVER_GIT_USER=""
ENV SERVER_GIT_PASSWORD=""

EXPOSE 8085


ENTRYPOINT ["/entrypoint.sh"]
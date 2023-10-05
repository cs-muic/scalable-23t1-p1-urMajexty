FROM amazoncorretto:11

WORKDIR /app

COPY ./scalable-ums-backend/target/ums-1.0.jar .

ENV MARIADB_ROOT_USERNAME=dev
ENV MARIADB_ROOT_PASSWORD=devpass
ENV UMS_DB_NAME=ums
ENV UMS_DB_USERNAME=dev
ENV UMS_DB_PASSWORD=devpass
ENV UMS_DB_PORT=3306
ENV UMS_DB_IP=db

ENV REDIS_HOST=redis

CMD ["java", "-jar", "ums-1.0.jar"]

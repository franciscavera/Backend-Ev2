FROM openjdk:11-oracle

COPY . .

RUN  ./gradlew task

RUN ./gradlew bootrun

COPY . .

COPY docker-entrypoint.sh /

RUN chmod +x docker-entrypoint.sh

ENTRYPOINT ["bash", "docker-entrypoint.sh"]

EXPOSE 1818
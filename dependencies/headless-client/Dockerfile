FROM openjdk:8

WORKDIR /usr/src/headless-client

RUN git clone https://github.com/emcmanus/toshi-headless-client.git . && git checkout fix-images

RUN ./gradlew ToshiHeadlessClientCapsule

CMD ["java", "-jar", "build/libs/toshi-headless-0.2.1-capsule.jar"]

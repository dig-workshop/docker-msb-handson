FROM gradle:8
COPY . /workspace
WORKDIR /workspace/api
RUN ./gradlew build
CMD [ "java", "-jar", "./build/libs/api-0.0.1-SNAPSHOT.jar" ]
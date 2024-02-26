FROM maven:3.8.3-openjdk-17 AS maven_build

COPY pom.xml /tmp/

COPY clamav-client-spec.yaml /tmp/

COPY src /tmp/src/

WORKDIR /tmp/
	
RUN mvn clean package -Dmaven.test.skip=true

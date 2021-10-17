# spring-grpc-client-server-demo
Spring Boot gRPC Client & Server Demo (Gradle)

## Step 1:

* Run Docker Container (MongoDB Database)

```bash
docker run -d -p 27017:27017 --name mongo_db \
      -e MONGO_INITDB_ROOT_USERNAME=admin \
      -e MONGO_INITDB_ROOT_PASSWORD=password \
      mongo
```

## Step 2:

* Go to project root folder

* Run command to generate java files from CardService.proto file

```bash
./gradlew build
```

## Step 3:

* Go to project root folder

* Run Command to start server

```bash
./gradlew spring-grpc-server-demo:bootRun
```

* Run Command to start client

```bash
./gradlew spring-grpc-client-demo:bootRun
```

## Step 4: 

* Import postman collection file and start tests
# Task 1

### Requirements

- Java
- Maven
- Spring Boot (Framework)
- MongoDB
- Docker

#### Dependencies

- spring-boot-starter-web
- spring-boot-starter-data-mongodb
- spring-boot-maven-plugin



## Rest  API Endpoints and Resources
Rest API Endpoint is mapped to `http://127.0.0.1:9090/servers/`

- PUT a server	`http://127.0.0.1:9090/servers/createServer`
Accept "server" object in body in json format.

- GET servers	`http://127.0.0.1:9090/servers/getServer`
Returns a list of "server" objects.

- GET server	by ID	`http://127.0.0.1:9090/servers/getServer?id=<ID>`
Returns a  "server" object matching with ID.

- GET servers	by Name	`http://127.0.0.1:9090/servers/getServer?name=<Nmae>`
Returns a list of "server" objects matching with Name.

- DELETE server	`http://127.0.0.1:9090/servers/deleteServer?id=<ID>`
Deletes a  "server" object matching with ID.

## RestController interface extends MongoRepository

```java
List<Server> findAll();
    
Optional<Server> findById(String Id);
    
void createOrUpdateServer(Server server);
    
void deleteServerById(String Id);
    
List<Server> findByName(String name);
```

### Using Postman

Run the following created collection to Test and consume the APIs

**NOTE:** *The above collection is created and tested for `http://127.0.0.1:9090/servers/` endpoint*

### Screenshots

**MongoDb URL and Server Port**

![Screenshot (4)](https://github.com/neeraj-git-workspace/Kaiburr_Assessment/assets/126611572/807054e4-1f4d-404c-8545-578d2f052bfb)


**SpringBoot Framework Started**

![Screenshot (5)](https://github.com/neeraj-git-workspace/Kaiburr_Assessment/assets/126611572/a1b72080-9e27-4328-90f8-1d15ec677f2a)


**POSTMAN - Create Server**

![Screenshot (6)](https://github.com/neeraj-git-workspace/Kaiburr_Assessment/assets/126611572/b2499168-893c-4096-a736-0b655a60a4b0)


**GET Server**

![Screenshot (7)](https://github.com/neeraj-git-workspace/Kaiburr_Assessment/assets/126611572/01a6f67e-13fa-4c0f-8432-1fb71be00fd4)


**GET Server By Id**

![Screenshot (8)](https://github.com/neeraj-git-workspace/Kaiburr_Assessment/assets/126611572/c547e385-5662-485b-aa16-6eb609697743)


**GET Server By Name**

![Screenshot (9)](https://github.com/neeraj-git-workspace/Kaiburr_Assessment/assets/126611572/246aea26-b333-4fa7-b119-201a8dc002ec)


**Delete Server**

![Screenshot (10)](https://github.com/neeraj-git-workspace/Kaiburr_Assessment/assets/126611572/33632b62-6a16-402f-a37e-514151e50da3)


**MongoDB Database**

![Screenshot (11)](https://github.com/neeraj-git-workspace/Kaiburr_Assessment/assets/126611572/1d7e925b-8853-4bc4-b6ef-cf22450143e1)









# usage

1. `git clone <URL>`
2. 'Run as Spring Boot Apps to build the app

# Testing API from Swagger UI
1. http://localhost:8080/swagger-ui/index.html
2. http://localhost:8080/v3/api-docs
# NOTE
If we are working with Java 17 and Spring Boot 3 and we have to expose all the services of our Rest API then we don't have to any config class or other stuff in Spring
Simply add this below dependency in your pom and that's it.

    <dependency>
			<groupId>org.springdoc</groupId>
			<artifactId>springdoc-openapi-starter-webmvc-ui</artifactId>
			<version>2.0.3</version>
		</dependency>

# Testing API from Browser
1. http://localhost:8080/car [GET] : No Body
2. http://localhost:8080/car [POST] with Body as shown below
   {
  "carId": 4,
  "carModel": "Audi C3",
  "carPrice": 6200000
   }
3. http://localhost:8080/car [PUT] with Body as shown below , CarId should be valid one
   {
  "carId": 4,
  "carModel": "Audi C3",
  "carPrice": 6200000
   }
4. http://localhost:8080/car/{carId} [DELETE] : No Body , CarId should be valid one

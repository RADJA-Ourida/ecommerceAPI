# ecommerceAPI
This projetc is a Spring Boot API for an ecommerce Web site. 


Requirements

- Install IntelliJ IDEA or any other integrated development environment (IDE)
- Install PgAdmin create a database "dbecommerce" then adapt the application.properties file to your own information.
- Import the project and download the dependencies if it's not done automaticly 
- Run the main class 
- Go to the browser and run "http://localhost:3000/api/products"


To dockerize the application : 
- Change the first row of the application.properties to : spring.datasource.url=jdbc:postgresql://postgresqldb:5432/dbecommerce
- In Ecommerce2ApplicatioTests.java, comment or remove the @SpringBootTest and the @Test 
- In the terminal of IntelliJ IDEA run : ./mvnw clean package -Dskiptest  -> a jar file will be added to /target
- Run docker compose up -> two docker images will be created in Docker that you can run.


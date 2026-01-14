As the first project I created a Spring Boot application using the Spring Initializr.
Dependencies added: Spring Web for processing HTTP requests, Thymeleaf for HTML templates, and Lombok for reducing boilerplate code. 

The next step was creating the first controller -- so a controller class annotated with the @Controller annotation.
A method annotated with the @GetMapping handles an HTTP GET request sent to localhost:8080. The @ResponseBody tells Spring that the method's return value should be sent directly to the HTTP response body, without searching for an HTML template.

![photo_5422352931274559849_x](https://github.com/user-attachments/assets/e20f4aa6-275a-400a-b085-70d412c94d17)

*localhost:8080*

In the next step, the application was extended to use the MVC pattern.
The controller passes data to the Model object, after which Thymeleaf processes the HTML template and substitutes the values ​​during rendering.
As a result, the browser receives a finished HTML page generated on the server side.

![photo_5422352931274559875_x](https://github.com/user-attachments/assets/b3092887-70bc-489c-82eb-697730345a9d)

*http://localhost:8080/greeting?name=Boba*

Hence, the application correctly handles HTTP requests, uses controllers, returns text responses and HTML views, and demonstrates the basic Spring MVC architecture.

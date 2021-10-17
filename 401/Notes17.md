
#  Spring Authorization

* **OAuth2** is an authorization framework that enables the application Web Security to access the resources from the client.

There are several samples building on each other, adding new features at each step:

* [simple](https://spring.io/guides/tutorials/spring-boot-oauth2/#_social_login_simple): a very basic static app with just a home page and unconditional login via Spring Boot’s OAuth 2.0 configuration properties.

* [click](https://spring.io/guides/tutorials/spring-boot-oauth2/#_social_login_click) : adds an explicit link that the user has to click to login.

* [logout](https://spring.io/guides/tutorials/spring-boot-oauth2/#_social_login_logout) : adds a logout link as well for authenticated users.

* [two-providers](https://spring.io/guides/tutorials/spring-boot-oauth2/#_social_login_two_providers) :  adds a second login provider so the user can choose on the home page which one to use.

* [custom-error](https://spring.io/guides/tutorials/spring-boot-oauth2/#_social_login_custom_error) : adds an error message for unauthenticated users, and a custom authentication based on GitHub’s API.


The rest of the page show us how to build a sample app doing various things with "social login" using OAuth 2.0 and Spring Boot. [Spring Boot and OAuth2](https://spring.io/guides/tutorials/spring-boot-oauth2/)
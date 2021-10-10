# Baeldung: Spring Request Mapping

1. **@RequestMapping Basics**:

* The HTTP method parameter has no default value that means if we didn't specify a value, it's going to map to any HTTP request.

* `@RequestMapping(value = "/ex/foos", method = RequestMethod.GET)` As we see in the `method` we can specify the type of HTTP requests by typing `RequestMethod.` and put the type of HTTP requests after the dot.

2. **RequestMapping and HTTP Headers**:

* The `@RequestMapping` annotation provides a header element to narrow down the request mapping based on headers present in the request. Also we can indicate multiple header values.

* The special use of this feature comes in the case of media types.

* Starting with Spring 3.1, the @RequestMapping annotation now has the produces and consumes attributes.

3. **RequestMapping With Path Variables**: 

@PathVariable is an annotation which indicates that a method parameter should be bound to a URI template variable. If the method parameter is `Map<String, String>` then the map is populated with all path variable names and values.

4. **RequestMapping With Request Parameters**: 

The `@RequestParam` annotation is used with `@RequestMapping` to bind a web request parameter to the parameter of the handler method.

The @RequestParam annotation can be used with or without a value. The value specifies the request param that needs to be mapped to the handler method parameter.

# Accessing Data with JPA

These notes fro how to build an application that stores Customer POJOs (Plain Old Java Objects) in a memory-based database.

* To generate a new project with the required dependencies (Spring Data JPA and H2 H2 Database).for *Gradle* users, visit the [Spring Initializr](https://start.spring.io/)

* The class is annotated with `@Entity`, indicating that it is a JPA entity. (Because no `@Table` annotation exists, it is assumed that this entity is mapped to a table of the class name.)

## Create an Application Class

* `@SpringBootApplication` : it is convenience annotation that use to auto-configuration, component scan and be able to define extra configuration on application class.

* `@EnableAutoConfiguration` : Tells Spring Boot to start adding beans based on classpath settings, other beans, and various property settings.

* `@Configuration` : Allow to register extra beans in the context or import additional configuration classes.

* `@ComponentScan` : Enable @Component scan on the package where the application is located.

# Baeldung: Comparing repositories

## CrudRepository

Typical CRUD functionality:

* `save(…)` – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch.

* `findOne(…)` – get a single entity based on passed primary key value.

* `findAll()` – get an Iterable of all available entities in database.

* `count()` – return the count of total entities in a table.

* `delete(…)` – delete an entity based on the passed object.

* `exists(…)` – verify if an entity exists based on the passed primary key value.

## JpaRepository

Methods in JpaRepository:

* `findAll()` – get a List of all available entities in database.

* `findAll(…)` – get a List of all available entities and sort them using the provided condition.

* `save(…)` – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch.

* `flush()` – flush all pending task to the database.

* `saveAndFlush(…)` – save the entity and flush changes immediately.

* `deleteInBatch(…)` – delete an Iterable of entities. Here, we can pass multiple objects to delete them in a batch.
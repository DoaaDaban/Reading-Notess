# Related Resources and Integration Testing

## The relations btween Entity classes:

### 1. One-to-Many Relationship

* A **One-to-Many** relationship refers to the relationship between two entities A and B in which one element of A may only be linked to many elements of B, but a member of B is linked to only one element of A.

* A one-to-many relationship between two entities is defined by using the `@OneToMany` annotation in Spring Data JPA.

### 2. One-to-One Relationship

* A **One-to-One** relationship refers to the relationship between two entities tables A and B in which only one element of A may only be linked to one element of B, and vice versa.

* A One-to-One relationship between two entities is defined by using the `@OneToOne` annotation in Spring Data JPA.

### 3. Many-to-Many Relationship

* A **Many-to-Many** relationship refers to the relationship between two entities A and B in which one element of A may only be associated with many elements of B and vice versa.

* A Many-to-Many relationship between two entities is defined by using the `@ManyToMany` annotation in Spring Data JPA.

### 4. Many-to-One Relationship

* A **Many-To-One** relationship represents a single-valued association where a collection of entities can be associated with the similar entity. Hence, in relational database any more than one row of an entity can refer to the similar rows of another entity.

* A Many-to-One relationship between two entities is defined by using the `@ManyToOne` annotation in Spring Data JPA.

## Integration Testing

Some integration test we can write:

1. Verify View Name

2. Verify Response Body

3. Send GET Request With Path Variable

4. Send GET Request With Query Parameters
# Web App Security

## Many to many relationships

* A **Many-To-Many** relationship is where more than one record in a table is related to more than one record in another table.

* A many-to-many relationship between two entities is defined by using the @ManyToMany annotation in Spring Data JPA.


The popular example of **Many-To-Many** relationship is the students and courses. A student can register for many courses and a course can include many students.

![Example about many to many realationship](https://www.baeldung.com/wp-content/uploads/2018/11/relation-entity-model-updated.png)

##  Security: a humorous overview

[This World of Ours](https://scholar.harvard.edu/files/mickens/files/thisworldofours.pdf)

The article includes stories and real-life examples about safety and the risk that we may be exposed to due to lack of protection.

The bottom line of this article is to avoid untrusted websites, and put strong passwords where they should include:

1. A mixture of lower and uppercase letters.

2. The password contains symbols.

3. Avoid common passwords such as putting date of birth as the password.

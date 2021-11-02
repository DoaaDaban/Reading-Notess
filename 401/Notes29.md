# Room

## Overview: Saving data with Room

We can save data in local database when the device cannot access the network by using **Room**.

Room benefits :

* Compile-time verification of SQL queries.

* Convenience annotations that minimize repetitive and error-prone boilerplate code.

* Streamlined database migration paths.

### Setup

We must put the folloeing dependencies (For Groovy users) in the `build.gradle` file to use Room:

```
dependencies {
    def room_version = "2.3.0"

    implementation "androidx.room:room-runtime:$room_version"
    annotationProcessor "androidx.room:room-compiler:$room_version"

    // optional - RxJava2 support for Room
    implementation "androidx.room:room-rxjava2:$room_version"

    // optional - RxJava3 support for Room
    implementation "androidx.room:room-rxjava3:$room_version"

    // optional - Guava support for Room, including Optional and ListenableFuture
    implementation "androidx.room:room-guava:$room_version"

    // optional - Test helpers
    testImplementation "androidx.room:room-testing:$room_version"

    // optional - Paging 3 Integration
    implementation "androidx.room:room-paging:2.4.0-alpha04"
}
```
### Primary components

There are three major components in Room:

1. The **database class**: its purpose is for holds the database and serves as the main access point for the underlying connection to your app's persisted data.

2. **Data entities**: represent tables in your app's database.

3. **Data access objects (DAOs)**: that provide methods that your app can use to query, update, insert, and delete data in the database.

## Defining entities in Room

To create a table in the database, we must annotate a class by using `@Entity`. A Room entity includes fields for each column in the corresponding table in the database, including one or more columns that comprise the primary key.

Some Entities annotations:

1. `@PrimaryKey`: Each Room entity must define a primary key that uniquely identifies each row in the corresponding database table.

2. `@ColumnInfo`: To give the column a name.

3. `@Ignore`: It is used If an entity has fields that you don't want to persist.

## Related entities in Room

Room Database enables us to create embedded objects. As sometimes we need to express objects as a cohesive whole in our database logic even if the object contains several fields. So, we can do that by using `@Embedded` annotation.

We can create relationships between objects, such as:

1. **one-to-one relationships**

2. **one-to-many relationships**

3. **many-to-many relationships**

## Accessing data with Room

Data Access Objects are used to access your application’s persisted data. They are a better and more modular way to access your database as compared to query builders or direct queries.

A Data Access Objects can be either an interface or an abstract class. If it’s an abstract class, it can optionally have a constructor that takes a RoomDatabase as its only parameter. Room creates each DAO implementation at compile time

We can perform multiple operations using Data Access Objects :

1. Insertion `@Insert`

2. Updation `@Update`

3. Deletion `@Delete`
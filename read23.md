# Room

## Save data in a local database using Room

Room provides the following benefits:

1. Compile-time verification of SQL queries.
2. Convenience annotations that minimize repetitive and error-prone boilerplate code.
3. Streamlined database migration paths.

### Primary components

1. The database class
2. Data entities
3. Data access objects

### Sample implementation

#### Data entity

Defining data using Room entities

* entities used to represent the objects that we want to store.Each entity corresponds to a table in the associated Room database.

* Anatomy of an entity: we define each Room entity as a class and annotated with @Entity

* Define a primary key:each room entity must have primary key and we annotate a single column with @PrimaryKey.

* Define a composite primary key:we define composite primary key by listing those columns in the primaryKeys property of @Entity:

##### Ignore fields

To ignore any feild we annotate them using @Ignore

#### Define relationships between objects

In the room we have two ways to define and query the a relationship between entities:

1. Intermediate data class
2. Multimap return types

In order to create embedded objects we use @Embedded annotation.

There are many relations between entities:

1. one-to-one relationship
2. one-to-many relationship
3. many-to-many relationship

#### Data access object (DAO)

Accessing data using Room DAOs

There are two types of DAO methods that define database interactions:

1. Convenience methods.(Insert,Update,Delete)
2. Query methods.

Special return types

1. Paginated queries with the Paging library
2. Direct cursor access

#### Database

In order to hold the database we need to creat a `AppDatabase` class,and this class define the configrations and save entry points and there is condtion must be satisfied:

1. annotated with a @Database
2. abstract class that extends RoomDatabase
3. must define an abstract method that has zero arguments and returns an instance of the DAO class

After defining the Primary components we can create an instance of the database.

## Resources used in this reading

1. [Save data in a local database using Room](https://developer.android.com/training/data-storage/room)
2. [Defining data using Room entities](https://developer.android.com/training/data-storage/room/defining-data)
3. [Define relationships between objects](https://developer.android.com/training/data-storage/room/relationships)
4. [Accessing data using Room DAOs](https://developer.android.com/training/data-storage/room/accessing-data#java)

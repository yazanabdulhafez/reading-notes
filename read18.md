# Web App Security

## Many to Many Annotation

* The assocation betweenEmployee class and Project classes is bidirectional.

* To map a many-to-many association, we use the @ManyToMany, @JoinTable and @JoinColumn annotations.

* The @ManyToMany annotation is used in both classes to create the many-to-many relationship between the entities.

* This association has two sides:

1. The owning side
2. The inverse side

* The @JoinTable is used to define the join/link table.

* The @JoinColumn annotation is used to specify the join/linking column with the main table

## This World of Ours

* This World of Ours by James M ickens its an essay talk about the security issues in a humorous overview ,and the solution for a security matters

* The solution to prvent our emails and accounts from hacking by create strong passwords and change them in short periods.

## Reading Resources

1. [Hibernate Many to Many Annotation](https://www.baeldung.com/hibernate-many-to-many)
2. [This World of Ours](https://scholar.harvard.edu/files/mickens/files/thisworldofours.pdf)

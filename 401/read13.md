#  Related Resources and Integration Testing

## Working with Relationships in
### Spring Data REST

### One-to-One Relationship

`
 @Entity
public class Library {
    @Id
    @GeneratedValue
    private long id;
    @Column
    private String name;
    @OneToOne
    @JoinColumn(name = "address_id")
    @RestResource(path = "libraryAddress", rel="address")
    private Address address;
    // standard constructor, getters, setters
}`

`@Entity
public class Address {
    @Id
    @GeneratedValue
    private long id;
    @Column(nullable = false)
    private String location;
    @OneToOne(mappedBy = "address")
    private Library library;
    // standard constructor, getters, setters
} 
`
### One-to-Many Relationship

`@Entity
public class Book {

    @Id
    @GeneratedValue
    private long id;
    
    @Column(nullable=false)
    private String title;
    
    @ManyToOne
    @JoinColumn(name="library_id")
    private Library library;
    
    // standard constructor, getter, setter
}
`

### Many-to-Many Relationship

`@Entity
public class Author {

    @Id
    @GeneratedValue
    private long id;

    @Column(nullable = false)
    private String name;

    @ManyToMany(cascade = CascadeType.ALL)
    @JoinTable(name = "book_author", 
      joinColumns = @JoinColumn(name = "book_id", referencedColumnName = "id"), 
      inverseJoinColumns = @JoinColumn(name = "author_id", 
      referencedColumnName = "id"))
    private List<Book> books;

    //standard constructors, getters, setters
}`

## Integration Testing in Spring

### Integration testing plays an important role in the application development cycle by verifying the end-to-end behavior of a system.

- ### [Integration Testing in Spring](https://www.baeldung.com/integration-testing-in-spring)

## Sources:
- ### [SpringDataREST](https://www.baeldung.com/spring-data-rest-relationships)


- # [spring-security-architecture](https://spring.io/guides/topicals/spring-security-architecture/)

## Spring security is framework used for securing Spring applications. It stands between client and application and gives possibility of configuring what data and functionalities are exposed to which users. Also, it handles common vulnerabilities

## Authentication and Access Control

### Authentication is any process by which a system verifies the identity of a user who wishes to access the system. Because access control is typically based on the identity of the user who requests access to a resource, authentication is essential to effective security


Spring Auth Cheat Sheet
Step 1: set up a user model and repo
Step 2: create a controller for that model
Step 3: UserDetailsServiceImpl implements UserDetailsService
gets a User from the database by username (make sure your repository has the method to make this easy!)
Step 4: ApplicationUser implements UserDetails
use IntelliJ to implement the methods; make the boolean ones all return true
Step 5: WebSecurityConfig extends WebSecurityConfigurerAdapter
• has a UserDetailsService
• passwordEncoder bean
Show more
<https://github.com/codefellows/seattle-java-401d2|codefellows/seattle-java-401d2>codefellows/seattle-java-401d2 | Added by GitHub






# Spring Auth Cheat Sheet
## Step 1: set up a user model and repo
## Step 2: create a controller for that model
## Step 3: UserDetailsServiceImpl implements UserDetailsService
gets a User from the database by username (make sure your repository has the method to make this easy!)
## Step 4: ApplicationUser implements UserDetails
use IntelliJ to implement the methods; make the boolean ones all return true
## Step 5: WebSecurityConfig extends WebSecurityConfigurerAdapter
has a UserDetailsService
passwordEncoder bean
configure AuthManagerBuilder
auth.userDetailsService(userDetailsService).passwordEncoder(passwordEncoder());
configure HttpSecurity
cors? csrf?
matchers for URLs that are allowed
ensure that login and signup URLs allowed; also consider homepage etc.
formLogin with login page set up
logout
```
    @Override
    @Bean
    public AuthenticationManager authenticationManagerBean() throws Exception {
        return super.authenticationManagerBean();
    }
```
## Step 6: registration page
create it w/ form
ensure it posts to a route your controller is ready for
check it's saving in the DB
```
    // maybe autologin?
    Authentication authentication = new UsernamePasswordAuthenticationToken(newUser, null, new ArrayList<>());
    SecurityContextHolder.getContext().setAuthentication(authentication);
```
## Step 7: login page
create it w/ form
ensure it posts to the route you specified in web config
try it out!
add to a template w/ things about the Principal


## Sources:

- ### [SpringAuthCheatSheet](https://github.com/codefellows/seattle-java-401d2/blob/master/SpringAuthCheatSheet.md)

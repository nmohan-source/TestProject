# TestProject
Spring boot project with openLDAP Authentcation

For spring security and  for ldap authentication added the following dependencies in pom.ml

<dependency>
		<groupId>org.springframework.boot</groupId>
		<artifactId>spring-boot-starter-security</artifactId>
</dependency>
<dependency>
		<groupId>org.springframework.ldap</groupId>
		<artifactId>spring-ldap-core</artifactId>
</dependency>
<dependency>
		<groupId>org.springframework.security</groupId>
		<artifactId>spring-security-ldap</artifactId>
</dependency>

To secure the web application, we need to create a configuration class which defines the authentication configuration.
It overrides the methods of WebSecurityConfigurerAdapter which implements the WebSecurityConfigurer interface.

We need to start the OpenLDAP server, and provide the URL,port and base domain details to establish a connection from our application.

### SpringBoot-WebSocket

### required
* Scala 2.1*
* JDK 1.8*
* Gradle 3.*
* Mysql 5.1*

![功能设计](https://github.com/scalad/WebSocket/blob/master/doc/image/function.png)

### technology

* Gradle
* Scala
* SpringBoot
* SpringSecurity
* Spring Data Jpa
* Redis


### configuration
`application.properties`
    
    #datasource
	spring.datasource.url = jdbc:mysql://localhost:3306/websocket
	spring.datasource.username = root
	spring.datasource.password = root
	spring.datasource.driverClassName = com.mysql.jdbc.Driver
	# Specify the DBMS
	spring.jpa.database = MYSQL
	# Show or not log for each sql query
	spring.jpa.show-sql = true
	# Hibernate ddl auto (create, create-drop, update)
	spring.jpa.hibernate.ddl-auto = update
	# stripped before adding them to the entity manager)
	spring.jpa.properties.hibernate.dialect = org.hibernate.dialect.MySQL5Dialect	
	# Server port
	server.port=80
	
### build

* git clone https://github.com/silence940109/WebSocket.git
* gradle bootRun
* http://localhost:8080/swagger-ui.html
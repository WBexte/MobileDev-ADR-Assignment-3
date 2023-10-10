## Status

The status for this AD is _accepted_

## Context

The development of the project will require a database to transfer and secure data.The success of our project is dependent on a reliable and efficient database system developed to fulfil the specific demands of students and educators. The requirements that we look for in a database
	**1.Data Privacy and Security**
		The database must be able to encrypt data in order to manage sensitive information discovered inside the school system, such as personal profiles, grades, and any future tests or assignments. 
	**2.Performance Optimization**
		The database must have the capabilities to handle large quantity of data with minimal impact on performance.  
	**3.Offline Mode**
		The database must be be available offline, databases are able to work with no connection to the sever by storing data locally. When students and teachers will be able to access certain features and data while having no internet connection, 
	**4.Active Directory interrogations**
		The database must be capable of integrating the system with an Active Directory system, allowing for proper access control for both students and staff. Both students and teachers will be able to log in to the program after roles and permissions are configured.


## Decision

MongoDB is an NoSQL database management system.NoSQL database systems are an alternative to standard SQL-based relational databases. MongoDB stores data in documents that use a JSON-like format to represent and interact with data.
	**1.Data Privacy and Security**
		MongoDB includes many feature that enhance the security in the application. With MongoDB Atlas or MongoDB Enterprise you can encrypt data to make it unreadable, there is even an option to add extra encryption for sensitive data. A audit framework is offered to log when changes to the configuration of the database are made.
	**2.Performance Optimization**
		MongoDB uses indexes to improve query performance, indexes are a special data structure that stores the value of a specific field and is ordered by that field. Ad Hoc allows MongoDB to perform searches without having to define a structure in the queries.
	**3.Offline Mode**
		MongoDB can gain the ability to use Offline First application, Offline First allows the  database to perform many operations when there is no internet connection through a local database. 
	**4.Active Directory interrogations**
		MongoDB uses LDAP to authenticate users and give them their respective role.  

## Consequences

In conclusion, the use of MongoDB as a database system response well with the projects objectives, MongoDB offers features for data privacy, offline mode and an active directory. MongoDB uses indexes and other feature to increase the amount of data being handled without impacting performance. The decision to use MongoDB comes with the following consequence:

**Performance levels and higher speed**
	MongoDB is built for speed. It enables indexing on any field in the documents, which can considerably improve query performance.
**Scalability**
	MongoDB uses horizontal scalability which allows the application to scale up without the need to change the code. 
**High Memory Usage** 
	MongoDB uses indexers to improve query performance however the lack of join functions leads to the duplication of data which takes up unnecessary space. 


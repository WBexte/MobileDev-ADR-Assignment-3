## Status

The status for this AD is _accepted_

## Context

Our project involves the development of a mobile and desktop application tailored for both students and professors. This application aims to provide a seamless experience on both iOS and Android platforms while ensuring high performance and robust security. Several key considerations guide our backend development
	**1.Data Security** 
		The backend should be able to encrypt data to be able to handle sensitive information that could be found within the school system such as personal profile ,  grades, and possible future test or homework.
	**2.Push Notifications** 
		The backend should integrate a function that allows the application to send notifications. This will keep the students informed about news that occur in their school/program/class, this will keep for miscommunication for deadlines or change in classrooms, etc.   
	**3.Active Directory interrogations**
		The backend would need to able to integrate the system into a Active Directory system, this will allow for correct access control for both student and employees. With roles and permissions set both students and teacher will be able to log in into the application.		

## Decision

Node.js is a server-side runtime environment that is ideal for developing the backend system mentioned in the case at hand for a mobile and desktop application geared towards students and education. Node.js has a provided libraries that offers security, real-time capabilities, and scalability needed to handle sensitive data, push notifications, and integration with external systems like Active Directory. Additionally, its cross-platform compatibility ensures a consistent experience across iOS, Android, and desktop devices.
**1.Data Security** 
	Node.js includes a large ecosystem of libraries and modules, including encryption and security components. Developers may use libraries like Crypto to create encryption techniques, assuring the safe storage and transport of sensitive data including user profiles, grades, and other protected data. 
**2.Push Notifications** 
	Node.js is well-known for its event-driven, non-blocking design, which makes it a good choice for dealing with real-time applications such as push notifications. Node.js can easily manage and dispatch alerts to mobile and desktop clients with libraries like Firebase Cloud Messaging (FCM) or WebSocket support, keeping students informed about essential modifications in their school or classes.
**3.Active Directory** 
	Node.js provides flexibility and versatility when it comes to interacting with multiple authentication systems, such as Active Directory. Passport.js and other libraries and packages may be used to construct authentication and access control methods that correspond to roles and permissions for both students and instructors. 

## Consequences

In conclusion, the use of Node.js as the backend language corresponds well with the project's objectives, providing the essential features for data security, real-time alerts, and Active Directory functions. This choice should make it easier to create a high-performance, secure, and user-friendly mobile and desktop application for students and academics.
The decision to use Node.js as the backend language has the following consequences:

**1.Easier Data Security**: Implementing data security features such as encryption becomes more manageable due to the availability of encryption libraries and the strong Node.js ecosystem.
    
**2.Efficient Push Notifications**: Node.js' event-driven architecture enables efficient handling of push notifications, ensuring that students receive timely updates about school-related events.

**3.Effective Active Directory Integration**: Integrating with Active Directory for access control becomes straightforward, allowing for secure user authentication and role-based permissions.
    
**4.Cross-Platform Compatibility**: Node.js' cross-platform compatibility ensures a consistent experience across iOS, Android, and desktop devices, simplifying development and maintenance efforts.

**5.Unstable API**: Node.js is constantly being updating and gaining new implications, the risk from not maintaining the application could lead to either the breaking of code or unexpected behaviour from the code or compatibility issues.   

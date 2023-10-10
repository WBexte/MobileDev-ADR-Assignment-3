# Defining User Roles and Permission

## Status

The status of this AD is *accepted*

## Context

Our team is developing a social media app for students on campus. The goal is to allow students to communicate with each-other, share class and club information, view and manage their schedules and view various clubs or events. Additionally, the app will allow professors to post information, class announcements and student grades.

For this, we need to properly define user roles, break down the granular user permission levels and acknowledge the use of third-party applications to ensure user privacy and consent of information usage.

## Decision

#### 1. Defining user roles:
1. System Administrator:
	- The System Administrator is a superuser with access to all permissions and are responsible for managing app content and/or user info.
2. Professor (end-user):
	- Professors hold an 'admin'-like role and are responsible for managing the content, grades, announcements and other miscellaneous content on the app for any classes they teach.
3. Student (end-user):
	- Students are able to consume the information on app. They can post content and message other users on the app. Additionally, they can manage their course schedule through the app as well as view their class information.
4. Club or Event Coordinator:
	- A club or event coordinator is responsible for managing any clubs or activity information on the app.

#### 2. Breaking down user permissions:
The app will utilize role-based access permissions which will prevent end-users from accessing information they are not supposed to (e.g., students accessing other student grades)

1. System Administrator:
	- The system administrator will have full permissions on the platform, as well as the ability to make edits to any information (student, professor, posts, etc.). They can also approve/deny any new posts on the platform that require manual review (i.e., new campus events, new clubs, etc.)
2. Professor:
	- Professors will be able to edit class information, post announcements to class boards, access all student grades for the classes they teach as well as post or make edits to the information, and lastly post course content to classes they teach.
3. Student:
	- Students will have access to view any classes they are currently registered in as well as post to discussion boards for the class. They will also be able to make edits to their schedule (i.e., enroll or drop courses), message other students and view events or club activities.
4. Club or Event Coordinator:
	- Club and Event coordinators will have edit permissions on the clubs and events section of the app. They will have the ability to create new clubs and events, post new announcements or information to the forum, invite members who are app users and delete/manage content. Any new event or activity will need to be approved by the system administrator.

#### 3. Central Authentication:
The application will utilize a central authentication system that will allow anyone with a student account for their school to log in using SSO. This will reduce the friction of sign-ups for users and increase app adoption.

#### 4. Third-party access and information sharing:
1. When users first downloads and log into the app, they will be required to read and accept the terms of service for using the app. This will acknowledge any third-party softwares (e.g., OneSignal) that are required for the proper function of the application, as well as any information that we will be sharing with said third-parties. 

#### 5. Access to Device Features:
1. The app may request permission to access some device features to provide a better user experience. These features may include push-notifications, location services and access to device storage. Once a user provides permission to access theses features, they will have full access to the application services.

## Consequences

##### Pros:
1. Defining distinct user roles ensures a smooth experience with the application and will prevent any issues arising with permission abuse or privacy breaches
2. Central authentication will greatly reduce friction for user-signups and boost adoption of the app
3. The use of third parties such as OneSignal will improve user experience and allow the team to introduce innovative features and experiences to the end-user.
##### Cons:
1. Some users may be hesitant to allow access to device features which will cause issues with app performance
2. There may be pushback from some users regarding data-sharing with third parties

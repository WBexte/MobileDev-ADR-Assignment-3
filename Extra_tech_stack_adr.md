## Status

The status of this AD is *accepted*

## Context

Our app will be dealing with sensitive information such as student grades and course information.  Because of this, we need to implement robust security practices to ensure user privacy is maintained.

## Decision

Implement robust security measures that safeguard user data, and ensure we are compliant with any data security and maintenance regulations.

#### 1. API Security
The social networking app will utilize third-party software such as CloudFlare to maintain API security. 
#### 2. Multi-Factor Authentication
Additionally, we will implement Auth0 and enforce mandatory 2-factor-authentication for accounts on the application.

#### 3. Proper Data Logging
The app will implement loggers to record user activity and quickly identify any security issues or data breaches.

#### 4. Role Based Access Control
As explored in a previous ADR, end-users will be assigned roles based on their relationship to the institution. Each role will be given specific permissions based on their responsibilities. Doing so will prevent unwanted access to sensitive data.

## Consequences

#### 1. Enhanced Data Security
Implemented robust practices will ensure there are no data breaches that leak sensitive or private information.
#### 2. User Trust and Compliance
Building trust with your userbase is important. If you have a positive reputation it will boost adoption of your product. Additionally, adhering to regulations will help avoid any legal issues in the future.
#### 3. Increased Development Time
Implementing robust security measures will take a lot of time and needs to be taken into consideration when creating a timeline for project deliverables.

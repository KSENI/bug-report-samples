# bug-report-samples
Bug report samples. No more, no less.

## [Web] All users receive the message, not only  group members

Precondition: Two accounts that have a group conversation, and another account that isn't in the group conversation. User1 - sender *credentials*,  user2 - expected receiver *credentials*, user3 - not is a group conversation, shouldn't receive the message *credentials*.

Steps: 
1. Open the chat with the user1 account
2. Open the service with the user2 account on the other browser or in incognito mode
3. Open the service with the user3 account on the third browser
4. Send the message with the user1 account

Expected result: 
User2 receives the notification and the message, but user3 doesn't receive the notification and the message.

Actual result: 
User2 and user3 receive the notifications and see the message from user1 on their chats list.

Environment: backend: *A*,  frontend: *B*

Attachments: *Video of a bug*

## [Security] The user can earn unlimited bonus points by taking the same survey several times

Precondition: The user has already taken a survey,  account example: *credentials*.

Steps:
1. Open *link*
2. Click the hamburger menu
3. Click 'My account'
4. Click 'Login'
5. Fill in the login and password
6. Click 'Log in' button
7. Open the DevTools inspector
8. Select 'Take a survey' button in the inspector
9. Remove class 'disabled ' in the inspector
10. Click 'Take a survey' button

Expected result: 
The backend has a limit for taking surveys and the user can't take the same survey twice and earn bonus points. 

Actual result: 
The user can take the same survey a lot of times if they delete the 'disabled' class on the DevTools.

Environment: backend: *A*, frontend: *B*

Attachments: *Video of a bug*

## [Mobile] The app crashes when the user taps *element name* on the home screen on Android 10

Steps:
1. Open the app
2. Skip the splash screen
3. Scroll to the *element name*
4. Tap on the *element name*

Expected result:
The user has access to the next screen

Actual result:
The app crashes

Environment: app version: *A*, device: *B*, OS: Android 10

Attachements: *crash report*, *video with steps*

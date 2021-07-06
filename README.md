
# Set up

- clone the repo
- open the dynamic links project 
- connect it with your Firebase project
- follow the instructions in the Firebase console (add an android app)
- in the code, modify :
    - in app/build.gradle : change the applicationId with yours
    - in mainFlavor, in resValue change the Dynamic Links URI prefix with the one set in the DynamicLinks section of Firebase
    - in MainActivity : change the DEEP_LINK_URL with your deeplink set in the DynamicLinks section of Firebase

# How to reproduce the issue

- build the project on an android emulator or phone
- launch the app and click on share button
- share the link via email
- on the Firefox browser (on your device), go to your mail website for example Gmail and sign in
- click on the link you received from the share


Firefox doesn't open your app => it redirects you to the app page on the play store website (not the app)

| | |
| ---- | ---- |
|![image](https://user-images.githubusercontent.com/50346870/124576015-326fca80-de4c-11eb-9654-9fac9b06a93a.png) | ![image](https://user-images.githubusercontent.com/50346870/124576032-36035180-de4c-11eb-9018-5bde3bba7184.png) |
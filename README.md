
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

Tested on emulator Pixel 4 Api30  

| click on Java | click on share | share by mail | send mail | open mail on firefox | redirects to play store page | ask to download it | 
| ---- | ---- | --- | ---- | --- | ---- | --- |
|![image](https://user-images.githubusercontent.com/50346870/124614938-103e7280-de75-11eb-9281-c70fa762d6e8.png) | ![image](https://user-images.githubusercontent.com/50346870/124615050-2a785080-de75-11eb-8449-cf93739413a3.png) | ![image](https://user-images.githubusercontent.com/50346870/124615108-395f0300-de75-11eb-80f6-4f8536542d4d.png) | ![image](https://user-images.githubusercontent.com/50346870/124615309-6dd2bf00-de75-11eb-99aa-1edcfde03b9f.png) | ![image](https://user-images.githubusercontent.com/50346870/124615657-c4d89400-de75-11eb-9570-28a410776000.png) |![image](https://user-images.githubusercontent.com/50346870/124576015-326fca80-de4c-11eb-9654-9fac9b06a93a.png) | ![image](https://user-images.githubusercontent.com/50346870/124576032-36035180-de4c-11eb-9018-5bde3bba7184.png) |

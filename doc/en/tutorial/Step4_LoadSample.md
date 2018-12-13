### Step 4:  Load React Native Sample from Github

1.	Open the Command prompt and navigate to your development workspace. Then run `git clone https://github.com/CPE-OAuth/servicestage-mobileapp-react-example.git`  

    If you are having issues cloning the project, you can instead visit the url and download the project as a zip.

2.	Change to `servicestage-mobileapp-react-example` directory using `cd {{path to}}/servicestage-mobileapp-react-example`

3.	Run `npm install` to install project dependency.  It may take some time to install all dependency.  Once completed, it shows a line similar to the below.  
![s3a.png](./imgs/s3a.png)  

4.	Run `npm install -g react-native-cli` to install react native client.  

5.  Change to `servicestage-mobileapp-react-example/android` folder.  Create a **local.properties** file.  In the file, it should contains the path to Android SDK.  For example,

```
    sdk.dir=C\:\\Users\\{{Your Username}}\\AppData\\Local\\Android\\Sdk
```

6.  Run `gradlew clean`.    

7.  Run `cd..` to go back.    

8.  Run the following command to verify bundling is ok.   

```
   react-native bundle --platform android --dev false --entry-file index.android.js --bundle-output android/app/src/main/assets/index.android.bundle --assets-dest android/app/src/main/res
```


  
  

# cordova-codepush

Installation of cordova

first install node.js

In your command-line on Windows:

    c:\> npm install -g cordova
In your terminal on Mac OS X/Linux:

    $sudo npm install -g cordova
    


1> Creating a new Cordova project

This simple example demonstrates how Cordova CLI can be used to create a myApp project with the camera plugin and run it for android platform:

    cordova create myApp com.myCompany.myApp myApp
    cd myApp
    cordova plugin add cordova-plugin-camera --save (optional)
    cordova platform add android --save
    cordova requirements android    
    cordova build android --verbose
    cordova run android - to install app on conmected devices.
    
    
    
2 Install the CodePush CLI

  Command -  npm install -g code-push-cli
  
  2.1 Create a CodePush account


    Command -  code-push register
    
  2.3 Register your app with the service
  
  
    code-push app add MyApp_android android react-native
    
        or
        
    code-push app add <MyApp_android> android cordova
    
    
    Release an app update
    
    
    code-push release-react <MyApp_android> <android/ios>
                or
                
    code-push release-cordova <MyApp_android> <android/ios>
    
    
    
  
  
  
        
        
    
    
    
    
    
    
    
    
    

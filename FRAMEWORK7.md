SOSHUB.INC DEVELOPERS 
--------------------------------------------------------------------------------------


## FRAMEWORK7 CONFIGURATION AND INSTALLATION
A free and open source framework to develop mobile, desktop or web apps with native look and feel.

--------------------------------------------------------------------------------------


INSTALLATION
  

framework7 CLI is an extremely powerful tool and the most recommended way to start Framework7 app development.

It allows to create project using different variants to choose:

Framework: Framework7 Core, Framework7-Vue, Framework7-React, Framework7-Svelte
Target platform: Web app, PWA or Cordova app
Starter template: Single View, Tabs, Split View

Custom color theme
Generate required icons and splash screen

Many more
 -- get started --
 
on your nodes command line interface type the following to get the framework7 CLI package

$npm i framework7-cli cordova -g

$framework7 create --ui



-----------------------------------------------------------------------------------



TASTE THE INSTALLATION 

  C:\Users\soshub>framework7 -h
Usage: index <command> [options]

Options:
  -V, --version                     output the version number
  -h, --help                        output usage information

Commands:
  create [options]                  Create a new Framework7 project
  assets|generate-assets [options]  Generate Framework7 app icons and splash screens
  cordova [args...]                 Cordova CLI

------------------------------------------------------------------------------------



## Framework7 CLI Options

## Framework7 app created with following options:

```
{
  "cwd": "C:\\Users\\Bk Millanzi\\Desktop\\sostabs",
  "type": [
    "pwa",
    "cordova"
  ],
  "name": "SOSHUB",
  "framework": "vue",
  "template": "tabs",
  "bundler": "webpack",
  "cssPreProcessor": false,
  "theming": {
    "customColor": true,
    "color": "#0057ff",
    "darkTheme": true,
    "iconFonts": true,
    "fillBars": false
  },
  "customBuild": false,
  "webpack": {
    "developmentSourceMap": true,
    "productionSourceMap": true,
    "hashAssets": false,
    "preserveAssetsPaths": false,
    "inlineAssets": true
  },
  "pkg": "soshub.hybrid.beta",
  "cordova": {
    "folder": "cordova",
    "platforms": [
      "ios",
      "android"
    ],
    "plugins": [
      "cordova-plugin-statusbar",
      "cordova-plugin-keyboard",
      "cordova-plugin-device",
      "cordova-plugin-inappbrowser",
      "cordova-plugin-file",
      "cordova-plugin-media",
      "cordova-plugin-safariviewcontroller"
    ]
  }
}
`



-----------------------------------------------------------------------------------------------------------------------

Set Up Framework7 Android and Ios Development

After install framework7 global time for both mobile and web development configuration with the following process below
i.Java installation and configuration(JDK)
ii.Gradle installation and configuration
iii.Android studio installation and configuration

------------------------------------------------------------------------------------------------------------------------
 
 /*********************************************** 
 *                                              * 
 *   JAVA INSTALLATION AND CONFIGURATION        *
 *                                              *       
 ***********************************************/                                                                                                                                                      
Java JDK INSTALLATION

i. Download JDK setup in java official site
ii. Open JDK file setup for installation
iii. Installation begin 
done it
Note: With this steps you will be able to install java JDK in your pc

Java JDK PATH Enviroment Configuration

i.Locate java folder in your machine eg:- go to local disk c:
ii.Open java folder and then inside java folder locate the bin folder
iii. Copy the path from there inside your bin folder(C:\Program Files\Java\jdk1.8.0_271\bin)

# This Pc Configuration After Path Copy
 After copy your path inside your java folder time to go to this pc to set configuration

  i. Right click in your computer i mean this pc for window 10 user
  ii.Go to properties
  iii.Go to Advanced system settings
  iv.Click enviroment variable
  v.Go to user variable and you will see a path then click path->edit->new, then paste your path ( C:\Program Files\Java\jdk1.8.0_271\bin) 
  iv.Click okay,now you have successfull configure your path enviroment

# Taste Your Java Path Enviroment

/***********************************************************************************************************
* open cmd(command prompt) then type the following commang                                                  *
*                                                                                                           *
* C:\Users\soshub>javac                                                                                     *            
* where possible options include:                                                                           *
*  -g                         Generate all debugging info                                                   *
*  -g:none                    Generate no debugging info                                                    *
* -g:{lines,vars,source}     Generate only some debugging info                                              *
*  -nowarn                    Generate no warnings                                                          *
*  -verbose                   Output messages about what the compiler is doing                              *   
*  -deprecation               Output source locations where deprecated APIs are used                        *
*  -classpath <path>          Specify where to find user class files and annotation processors              *
*  -cp <path>                 Specify where to find user class files and annotation processors              *
*  -sourcepath <path>         Specify where to find input source files                                      *
*  -bootclasspath <path>      Override location of bootstrap class files                                    *
*  -extdirs <dirs>            Override location of installed extensions                                     *
*  -endorseddirs <dirs>       Override location of endorsed standards path                                  *
*  -proc:{none,only}          Control whether annotation processing and/or compilation is done.             *
*  -processor <class1>[,<class2>,<class3>...] Names of the annotation processors to run; bypasses default   *
*  -processorpath <path>      Specify where to find annotation processors                                   *
*  -parameters                Generate metadata for reflection on method parameters                         *
*  -d <directory>             Specify where to place generated class files                                  *
*  -s <directory>             Specify where to place generated source files                                 *
*  -h <directory>             Specify where to place generated native header files                          *
*                                                                                                           *
* Done Success Configure your java(JDK) in your Enviroment                                                  *
*                                                                                                           *
************************************************************************************************************/
  
ERROS OCCUR IN YOUR CONFIGURATION HOW TO FIX

1.Wrong path location: This will produce an errors in your enviroment especially when you try to run javac to taste

/*******************************************************************************************
*                                                                                          *
*   ERROR'S OUTPUT RESULT                                                                  *
*    C:\Users\soshub>javac                                                                 *
*   'javac' is not recognized as an internal or external command,                          *      
*     operable program or batch file.                                                      *                                    
*                                                                                          *
*  NOTE:The error try to tell us the java(JDK) have not configured collect in your machine *    
*          FIXED APPLY THIS BELOW                                                          *
*          C:\Program Files\Java\JDK0_271\bin                                              *
*******************************************************************************************/
2.This is An error C:\Program Files\Java\jdk1.8.0_271\
This kind of error occur when you are compile your project example you have a set up for android development enviroment and then try to run to see your output,remember when your are execute your code before a compile try to check all project the first step it's to check your JDK path envrioment and this will happen an error occur and stop all building process for project 
NOTE:This kind of error will not appear when you are taste your java path enviroment

How To fix 
here is the solution and very easy to fix it okay 
The problen it's your path you need to put root folder of bin remember this (C:\Program Files\Java\jdk1.8.0_271\) dont have it

/***********************************************
*          FIXED APPLY THIS                    *
*       C:\Program Files\Java\jdk1.8.0_271\bin *
*                                              *
***********************************************/

    DONE JAVA(JDK) INSTALLATION AND CONFIGURATION SECTION
--------------------------------------------------------------------------
   
    
    
   /************************************************
   *                                               *
   * ANDROID STUDIO INSTALLATION AND CONFIGURATION *
   *                                               *
   ************************************************/


   INSTALLATION
   ----------------------------------------------------------------------
   i.Download Android studio via official website
   ii.Open the download file 
   iii.Then Installation process take press
   iV.Click finish then done it 

   Installation process successfull
  -----------------------------------------------------------------------


  
  ADDING IMPORTANT FEATURES IN YOUR IDE
  
  i.Open android studio.
  ii.Download AVD by click create virtual development icon to create it.
  iii.Taste your emmulattor after downloaded,run it!
  iv.Open setting in IDE and then find SDK path location in your android studio copy  it
  v.Or you could copy in your pc example in my pc(C:\Users\soshub\AppData\Local\Android\Sdk) find the path  and copy it
  
  Path Enviroment successful
  ------------------------------------------------------------------------
  
  APPLY PATH ENVIROMENT PROCEDURE SDK
  
  After copy your path inside your java folder time to go to this pc to set configuration
  i. Right click in your computer i mean this pc for window 10 user
  ii.Go to properties
  iii.Go to Advanced system settings
  iv.Click enviroment variable
  v.Go to user variable and click new, inside variable name write ANDROID-HOME
  iv.Inside variable value paste your android sdk path((C:\Users\soshub\AppData\Local\Android\Sdk))
  iiv.Click okay
 SDK Path Enviroment successful

 ----------------------------------------------------------------------------



 TASTE ENVIROMENT 

 I.Open cmd 
 ii.type android to check if it is working or publish some error's
 
 When your paste the android command in cmd(command prompt),The follwoing result will occur
 
C:\Users\soshub>android
**************************************************************************
The "android" command is deprecated.
For manual SDK, AVD, and project management, please use Android Studio.
For command-line tools, use tools\bin\sdkmanager.bat
and tools\bin\avdmanager.bat
**************************************************************************




Invalid or unsupported command ""

Supported commands are:
android list target
android list avd
android list device
android create avd
android move avd
android delete avd
android list sdk
android update sdk

iii.Now it's working 100%

-----------------------------------------------------------------------------------




ERRORS AND SOLUTION HOW TO FIX IT
Most problem occur when you are copied the wrong path location of your SDK,

/***********************************************************************************************************
                                                                                                           *
                ERROR OUTPUT RESULT                                                                        *
*    C:\Users\soshub>javac                                                                                 *
*   'android' is not recognized as an internal or external command,                                        *      
*     operable program or batch file.                                                                      *
This will produce an error to avoid it's better to get the right path configuration location in your pc    *
***********************************************************************************************************/


            SOLUTION 
              i.Copy the right sdk path 
              Path location example  C:\Users\soshub\AppData\Local\Android\Sdk
              type android in your cmd command line 

              output result after runing android in your command prompt interface
              android list target
android list avd
android list device
android create avd
android move avd
android delete avd
android list sdk
android update sdk

                     DONE IT ANDROID STUDIO IDE INSTALLATION AND CONFIGURATION



*********************f***********************************************************************************/




   GRADLE INSTALLATION AND CONSFIGURATION

   /************************************************
   *                                               *
   * GRADLE INSTALLATION AND CONFIGURATION         *
   *                                               *
   ************************************************/

   INSTALLATION

   ----------------------------------------------------------------------------------------------------
   i.Download Gradle via official website  https://gradle.org 
   ii.Unzip gradle file  
   iii.Copy the gradle folder
   iV.Paste to your local disk c exapmle (C:\) 
   v. Done it

   Installation process successfull

  -----------------------------------------------------------------------------------------------------





  APPLY PATH ENVIROMENT PROCEDURES 
  
  After paste the gradle folder to local disk then we need to set path in our path enviroment
  i.open gradle folder and open bin folder inside gradle folder
  ii.Copy gradle path in your bin folder inside your gradle folder (C:\gradle-4.0\bin)
  iii. After copy then Right click in your computer i mean this pc for window 10 user
  iv.Go to properties
  v.Go to Advanced system settings
  vi.Click enviroment variable
  vii.Go to user system variable->path->edit->new, paste your path
  viii.Click okay 
  
 GRADLE Path Enviroment successful

 -----------------------------------------------------------------------------------------------------




TASTE ENVIROMENT 

 I.Open cmd 
 ii.type gradle -v to check if it is working or publish some error's
 
 When your paste the gradle -v command in your cmd(command prompt),The follwoing result will occur
/***************************************************************************
C:\Users\soshub>gradle -v                                                  *
                                                                           *
------------------------------------------------------------               *
Gradle 6.7                                                                 *
------------------------------------------------------------               *
                                                                           *
Build time:   2020-10-14 16:13:12 UTC                                      *
Revision:     312ba9e0f4f8a02d01854d1ed743b79ed996dfd3                     *
                                                                           *
Kotlin:       1.3.72                                                       *
Groovy:       2.5.12                                                       *
Ant:          Apache Ant(TM) version 1.10.8 compiled on May 10 2020        *
JVM:          1.8.0_271 (Oracle Corporation 25.271-b09)                    *
OS:           Windows 10 10.0 amd64                                        *
***************************************************************************/

Now it's working ,you will see gradle version in your command line interface 
---------------------------------------------------------------------------------------------------





ERRORS AND SOLUTION HOW TO FIX IT
Most problem occur when you are copied the wrong path location of your SDK,

/***********************************************************************************************************
                                                                                                           *
                ERROR OUTPUT RESULT                                                                        *
*    C:\Users\soshub>gradle -v                                                                             *
*   'android' is not recognized as an internal or external command,                                        *      
*     operable program or batch file.                                                                      *
This will produce an error to avoid it's better to get the right path configuration location in your pc    *
***********************************************************************************************************/




            SOLUTION 
              i.Copy the right gradle path 
              Path location example  (C:\gradle-4.0\bin)
              type gradle -v in your cmd command line interface 

              output result after runing gradle -v in your command prompt interface

           C:\Users\soshub>gradle -v                                       *
                                                                           *
------------------------------------------------------------               *
Gradle 6.7                                                                 *
------------------------------------------------------------               *
                                                                           *
Build time:   2020-10-14 16:13:12 UTC                                      *
Revision:     312ba9e0f4f8a02d01854d1ed743b79ed996dfd3                     *
                                                                           *
***************************************************************************/                                                                           







         DONE IT GRADLE INSTALLATION AND CONFIGURATION

*********************f***********************************************************************************/
             


             
             
               GETTING STARTED





##        IN YOUR CMD : run the following command below

##         C:\Users\soshub>framework7 create ui   


## note: create ui it's will provides the user interface(UI) for user to customize the project and it's very simple 

## Run the following below npm scripts in your command line interface 
Note: for mobile :- npm run cordova-android
## NPM Scripts

* 🔥 `start` - run development server
* 🔧 `dev` - run development server
* 🔧 `build-dev` - build web app using development mode (faster build without minification and optimization)
* 🔧 `build-prod` - build web app for production
* 📱 `build-dev-cordova` - build cordova app using development mode (faster build without minification and optimization)
* 📱 `build-prod-cordova` - build cordova app
* 📱 `build-dev-cordova-ios` - build cordova iOS app using development mode (faster build without minification and optimization)
* 📱 `build-prod-cordova-ios` - build cordova iOS app
* 📱 `cordova-ios` - run dev build cordova iOS app
* 📱 `build-dev-cordova-android` - build cordova Android app using development mode (faster build without minification and optimization)
* 📱 `build-prod-cordova-android` - build cordova Android app
* 📱 `cordova-android` - run dev build cordova Android app



## WebPack

There is a webpack bundler setup. It compiles and bundles all "front-end" resources. You should work only with files located in `/src` folder. Webpack config located in `build/webpack.config.js`.

Webpack has specific way of handling static assets (CSS files, images, audios). You can learn more about correct way of doing things on [official webpack documentation](https://webpack.js.org/guides/asset-management/).

## PWA

This is a PWA. Don't forget to check what is inside of your `service-worker.js`. It is also recommended that you disable service worker (or enable "Update on reload") in browser dev tools during development.

## Cordova

Cordova project located in `cordova` folder. You shouldn't modify content of `cordova/www` folder. Its content will be correctly generated when you call `npm run cordova-build-prod`.
## Assets

Assets (icons, splash screens) source images located in `assets-src` folder. To generate your own icons and splash screen images, you will need to replace all assets in this directory with your own images (pay attention to image size and format), and run the following command in the project directory:

```
framework7 assets
```


Or launch UI where you will be able to change icons and splash screens:

```
framework7 assets --ui
```

## Documentation & Resources

* [Framework7 Core Documentation](https://framework7.io/docs/)
* [Framework7 Vue Documentation](https://framework7.io/vue/)


* [Framework7 Icons Reference](https://framework7.io/icons/)
* [Community Forum](https://forum.framework7.io)

## Support Framework7

Love Framework7? Support project by donating or pledging on patreon:
https://patreon.com/vladimirkharlampidi
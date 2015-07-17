# Here Maps Android Example application

## Getting the SDK

You have to create an account at [Here website](https://developer.here.com/myapps/create/choose-plan#/) and create a new app in order to obtain your `app_id` and `app_code` at [you app's page](https://developer.here.com/myapps).

## Add Libraries to Your Project

In order to execute the application, you must add the required HERE SDK resources as follows:

1. From the directory where you downloaded the `HERE SDK`, copy the contents of the `HERE-sdk/libs/` folder, to your project's `app/app/libs/` folder (the same folder as the src).

2. copy the contents of the `HERE-sdk/libs/armeabi-v7a` folder to your project's `app/src/main/jniLibs/armeabi` folder. You will need to create the jniLibs and armeabi subfolders.

3. download the JTS Topology Suite (version 1.13 or later) from [http://sourceforge.net/projects/jts-topo-suite/](http://sourceforge.net/projects/jts-topo-suite/), extract its contents, and add the `jts-.jar` library into the `libs/` folder of your `Eclipse` project.

	Directory structure should be something like that:

	```
		├───libs
		│	 	gson-2.3.1.jar
		│	    HERE-sdk.jar
		│	    HERE-sdk.jar.properties
		│	    jts-1.13.jar
		└───src
		    └───main
		        ├───java
		        │   └───com
		        │       └───here
		        │           └───android
		        │               └───tutorial
		        │                   └───basicmap
			    ├───jniLibs                                                     
			    │   └───armeabi                                                 
			    │           libc++_shared.so                                    
			    │           libCertResourcesPkg.so                              
			    │           libcrypto.so                                        
			    │           libLohitIndicFontPkg.so                             
			    │           libMapsEngineResourcePkg.so                         
			    │           libMAPSJNI.so                                       
			    │           libNanumGothicFontPkg.so                            
			    │           libPureArabicFontPkg.so                             
			    │           libPureChineseFontPkg.so                            
			    │           libPureIndicSouthFontPkg.so                         
			    │           libPureThaiFontPkg.so                               
			    │           libSdkResourcePkg.so                                
			    │           libssl.so      
			    │                                     
		        └───res
		            ├───drawable-mdpi
		            ├───layout
		            ├───menu
		            └───values
	```

Result: Your project will be able to make use of APIs from the `HERE SDK`.

## Automatically adding the dependencies

In order to automatically include your libs dependencies, you should put the following code into your build.gradle:

```json
	dependencies {
	    compile fileTree(dir: 'libs', include: ['*.jar'])
	}
```

## Resources & docs

[Creating a Simple Application Using the HERE SDK](https://developer.here.com/mobile-sdks/documentation/android/topics/app-simple.html)

# Here Maps Android Example application


## Add Libraries to Your Project

In order to execute the application, you must add the required HERE SDK resources as follows:

1.  From the directory where you installed the `HERE SDK`, copy the contents of the `HERE-sdk/libs/` folder, except `HERE-sdk-javadoc.jar`, to your project's `libs/` folder.

2.  Next, download the JTS Topology Suite (version 1.13 or later) from [http://sourceforge.net/projects/jts-topo-suite/](http://sourceforge.net/projects/jts-topo-suite/), extract its contents, and add the `jts-_.jar_` _library into the `libs/` folder of your `Eclipse` project._

4.  _If you plan on extending this application with `HERE Places` or Routing functionality, add the `google-gson` library (release 2.2.4 or a compatible version) into your project. One way to do this is to download the `google-gson-`_-release.zip file from [https://code.google.com/p/google-gson/](https://code.google.com/p/google-gson/), unzip the ZIP archive, and then copy the `gson-_.jar_` _(not `gson-`_-sources.jar or `gson-*-javadoc.jar`) into your project `libs/` folder. The `google-gson` library is required for these operations.

5.  In your `Eclipse` project's `libs/` folder, select and right-click on these three `.jar` files and select <span class="menucascade"><span class="uicontrol">Build Path` > <span class="uicontrol">Add to Build Path``.

Result: Your project will be able to make use of APIs from the `HERE SDK`.

Note:` Performing these steps should also link Javadoc files to the SDK library. If Javadoc does not appear in `Eclipse`, please close and re-open your `Eclipse` project. If you would like to change the location of the docs folder, update the `HERE-sdk.jar.properties` file in the libs folder to match the docs folder location.</div>


## Resources & docs

[Creating a Simple Application Using the HERE SDK](https://developer.here.com/mobile-sdks/documentation/android/topics/app-simple.html)

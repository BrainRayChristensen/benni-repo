# Benni

# Instructions


1. Clone or download this repo.
2. In your project, go to the top, click file, click new and then click on New Module...


<img src="https://github.com/BrainRayChristensen/benni-repo/blob/master/instructionImages/img1.png" width="300" alt="instruction image">  


3. Scroll down, and click "Import .JAR/.AAR Package" and click next.  
4. Input the file path for where your downloaded benni-debug.aar and click finish.  
There should now be a benni-debug module in your project.
5. In order for your app to use the Benni library, you must import it into the module. This is done by right clicking on the module you want to use it in (most likely app) and clicking on open module settings then opening the dependencies tab and adding a module dependency for benni-debug.

<img src="https://github.com/BrainRayChristensen/benni-repo/blob/master/instructionImages/img3.png" width="250" alt="instruction image">  


6. Because the module depends on other libraries, the module that uses Benni must import those libraries. Open your top level build.gradle and add `maven { url "https://jitpack.io" }` inside the allprojects and repositories section. It should look something like this:

<img src="https://github.com/BrainRayChristensen/benni-repo/blob/master/instructionImages/img2.png" width="300" alt="instruction image">  


7. Next, open the `build.gradle` file in the module you want to use benni in and add `implementation 'com.github.felHR85:UsbSerial:4.5.2'` to the list of dependencies.


<img src="https://github.com/BrainRayChristensen/benni-repo/blob/master/instructionImages/img4.png" width="300" alt="instruction image">  

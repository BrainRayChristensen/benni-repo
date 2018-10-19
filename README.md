# Benni

# Instructions


1. Download the .aar file
2. In your project, go to the top, click file, click new and then click on New Module...


<img src="https://github.com/BrainRayChristensen/benni-repo/blob/master/instructionImages/img1.png" width="300" alt="instruction image">  


3. Scroll down, and click "Import .JAR/.AAR Package" and click next.  
4. Input the file path for where your downloaded benni-debug.aar and click finish.  
There should now be a benni-debug module in your project.
5. Because the module depends on other libraries, the module that uses it must import it. Open your top level build.gradle and add `maven { url "https://jitpack.io" }` inside the allprojects and repositories section. It should look something like this:

<img src="https://github.com/BrainRayChristensen/benni-repo/blob/master/instructionImages/img2.png" width="300" alt="instruction image">  

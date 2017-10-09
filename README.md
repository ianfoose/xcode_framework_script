# Xcode Framework Scripts
Script for Xcode run phases to create a universal framework or cleanup a universal framework project.

## Use

* In an Xcode Framework project add a new 'Agregate' target
* Add a 'Run Phase' 
* Paste either the clean up or merge script into the new run phase

### Merge Script Setup

Either copy and paste script into a run phase or  

make script executable and add path in run phase.  

Example: ```${SRCROOT}/script.sh```

### Cleanup Script

The cleanup script is used when submitting to the App Store, it removes the simulator binaries from the 'fat' framework, only works if bitcode support is disabled.

### Objective-C 

Make sure all .h classes are made 'public' and not set to project.

Also be sure to import all .h classes in the file ```<FRAMEWORKNAME>.h```

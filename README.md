# Xcode Framework Scripts
Script for Xcode run phases to create a universal framework or cleanup a universal framework project.


## Use

* In an Xcode Framework project add a new 'Agregate' target
* Add a 'Run Phase' 
* Paste either the clean up or merge script into the new run phase

### Merge Script Setup

Be sure to rename the 'Framework Name' to the name of your framework target

```bash
FRAMEWORK_NAME="SampleFramework"
```

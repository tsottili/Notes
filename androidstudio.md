##To use local .aar file in Android Studio project: 

### Steps:

1) copy filename.aar in project_dir/module_dir/libs subfolder

2) edit build.gradle file adding:
```
repositories {
    flatDir {
       dirs 'libs'
    }
}

dependencies {
    compile(name:'filename', ext:'aar')
}
```
3) Add some synch-build step... 

###flatdir Gradle documentation
https://docs.gradle.org/current/userguide/dependency_management.html#sec:flat_dir_resolver

##To use local .aar file in Android Studio project: 

### Steps:

1) copy filename.aar in <project>/<module>/libs subfolder
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
###flatdir Gradle documentation
https://docs.gradle.org/current/userguide/dependency_management.html#sec:flat_dir_resolver

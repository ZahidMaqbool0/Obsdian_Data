

# Jcenter Issue
BUILD FAILED in 13m 11s
error Failed to install the app. Command failed with exit code 1: gradlew.bat app:installDebug -PreactNativeDevServerPort=8081 FAILURE: Build failed with an exception. * ***==Where: Build file 'C:\zahid maqbool data\paragon\node_modules\@react-native-community\audio-toolkit\android\build.gradle==***' line: 4 * What went wrong: A problem occurred evaluating project ':react-native-community_audio-toolkit'. > Could not find method ==**jcenter**()== for arguments [] on repository container of type org.gradle.api.internal.artifacts.dsl.DefaultRepositoryHandler. * Try: > Run with --stacktrace option to get the stack trace. > Run with --info or --debug option to get more log output. > Run with --scan to get full insights. > Get more help at https://help.gradle.org. BUILD FAILED in 13m 11s.
info Run CLI with --verbose flag for more details.

```
when this top given error is show we simple enter the bottom given line
 google()
 mavenCentral()
 
 and we must remove the bottom given line
 
 jcenter()
 
```
# Other modules top given with same issue 

```
1. node_modules\@react-native-community\audio-toolkit\android\build.gradle
2. node_modules\@react-native-community\masked-view\android\build.gradle
3. node_modules\react-native-navigation-bar-color\android\build.gradle
4. node_modules\react-native-select-contact\android\build.gradle
```

# Error: Exception in HostObject::get pop 'RNCallKeep'
in this error the emulator show the red screen and this error show in screen Error: Exception in HostObject::get pop 'RNCallKeep' we follow the bottom given steps. and comment the 2 difrent method in bottom given path.

file path
```
node_modules\react-native-callkeep\android\src\main\java\io\wazo\callkeep\RNCallKeepModule.java
```

Comment bottom given methods 1
```java
    @ReactMethod

    public void startCall(String uuid, String number, String callerName) {

        this.startCall(uuid, number, callerName, false, null);

    }
```

Comment bottom given methods 2
```java
    @ReactMethod

     public void displayIncomingCall(String uuid, String number, String                 callerName) {

         this.displayIncomingCall(uuid, number, callerName, false, null);

     }
```


# Error: BackHandler
in bottom given path we comment the bottom given lines in bottom given methods.

file path
```
node_modules\react-native-modalbox\index.js
```

we comment the bottom given lines in this method. ==*componentWillUnmount()*==
```javascript
 //if (this.props.backButtonClose && Platform.OS === 'android')
//   BackHandler.removeEventListener('hardwareBackPress', this.onBackPress);
```
we comment the bottom given lines in this method. ==*close()==
```javascript
 // if (this.props.backButtonClose && Platform.OS === 'android')
//   BackHandler.removeEventListener('hardwareBackPress', this.onBackPress);
```


# Error: TypeError: ref.current.unstable_getBoundingClientRect is not a function 
Error
```error
TypeError: ref.current.unstable_getBoundingClientRect is not a function
```

Error resign is: application after login stuck.
```error
BottomSheet
BottomSheetHandleContainerComponent

```

bottom given path this line is ***==newArchEnabled=true**==* we write the false in this line ***==newArchEnabled=false==*** 







huhh
kjjggg
jggg
hh

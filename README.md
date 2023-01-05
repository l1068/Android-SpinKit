# Android-SpinKit (Fork)

### Gradle Dependency

1. Add it in your root build.gradle at the end of repositories:

   ```groovy
   allprojects {
	   repositories {
		   ...
		   maven { url 'https://jitpack.io' }
	   }
   }
   ```

2. Add the dependency

    ```groovy
    dependencies {
        implementation 'com.github.l1068:Android-SpinKit:master'
    }
    ```

   See for versions at [JitPack](https://jitpack.io/#l1068/Android-SpinKit)


## Usage
- Xml

 ```xml
<com.github.ybq.android.spinkit.SpinKitView
     xmlns:app="http://schemas.android.com/apk/res-auto"
     android:id="@+id/spin_kit"
     style="@style/SpinKitView.Large.Circle"
     android:layout_width="wrap_content"
     android:layout_height="wrap_content"
     android:layout_gravity="center"
     app:SpinKit_Color="@color/colorAccent" />         
```
 
- ProgressBar

 ```java
ProgressBar progressBar = (ProgressBar)findViewById(R.id.progress);
Sprite doubleBounce = new DoubleBounce();
progressBar.setIndeterminateDrawable(doubleBounce);
```

## Style
> 
 ```xml
@style/SpinKitView
@style/SpinKitView.Circle
@style/SpinKitView.Large
@style/SpinKitView.Small
@style/SpinKitView.Small.DoubleBounce   
 ```

## Acknowledgements
- [SpinKit](https://github.com/tobiasahlin/SpinKit).

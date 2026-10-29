PAGE 1
ANDROID PRACTICAL JOURNAL
             Module I & Module II
    Prepared from the supplied Android practical PDF

================== PAGE BREAK ==================

PAGE 2
Index â€“ Click a Practical to Navigate
Module I: Android Fundamentals & UI Design
Practical 1: Develop a simple "Hello World" Android application demonstrating project creation, Android
Studio interface, Android components, AVD creation, and application execution.

Practical 2: Develop an Android application demonstrating the use of Programming Resources (colors.xml,
themes.xml, strings.xml, dimens.xml, drawable resources) and apply them in UI components.

Practical 3: Develop an Android application demonstrating complete Activity Lifecycle methods and analyze
execution using Logcat.

Practical 4: Develop an Android application to create and integrate a Fragment and demonstrate Fragment
lifecycle methods.

Practical 5: Develop an Android application implementing Fragment-based UI navigation between multiple
screens.

Practical 6: Develop an Android application demonstrating communication between Activity and Fragment.

Practical 7: Develop an Android application using LinearLayout (Horizontal and Vertical) to design structured
UI.

Practical 8: Develop an Android application using RelativeLayout to align UI components dynamically.

Practical 9: Develop an Android application using TableLayout to design a structured Login/Registration
Form.

Practical 10: Develop an Android application using ScrollView to display long scrollable content.

Practical 11: Develop an Android application using AbsoluteLayout demonstrating fixed positioning.

Practical 12: Develop an Android application using FrameLayout to overlay UI elements.

Practical 13: Develop an Android application using ListView with ArrayAdapter and implement item click
handling.

Practical 14: Develop an Android application using GridView with Custom Adapter

Practical 15: Develop an Android application implementing RecyclerView as a modern alternative to
ListView.

Module II: Android System Components & Data Handling
Practical 1: Develop an Android application implementing AppBar (Toolbar) and Options Menu.

Practical 2: Develop an Android application demonstrating AlertDialog and custom DialogFragment.

Practical 3: Develop an Android application implementing contextual menus and popup menus.

Practical 4: Develop an Android application implementing Explicit and Implicit Intents.

Practical 5: Develop an Android application demonstrating Event Handling using Listeners (OnClick,
OnLongClick, etc.).

Practical 6: Develop an Android application using Adapters to populate Spinner or ListView dynamically.

================== PAGE BREAK ==================

PAGE 3
Practical 7: Develop an Android application implementing Started and Bound Services.

Practical 8: Develop an Android application implementing Notifications using Notification Manager.

Practical 9: Develop an Android application implementing Static and Dynamic Broadcast Receivers.

Practical 10: Develop an Android application implementing SQLite database CRUD operations.

Practical 11: Develop an Android application integrating SQLite with ListView or RecyclerView.

Practical 12: Develop an Android application to fetch and parse JSON data from a web

Practical 13: Develop an Android application demonstrating Threads and Handlers for background
processing.

Practical 15: Develop an Android application implementing Runtime Permissions and security handling in
AndroidManifest.xml.

================== PAGE BREAK ==================

PAGE 4
[No extractable text on this page.]

================== PAGE BREAK ==================

PAGE 5
Module 1 â€“ Practical 1
Develop a simple "Hello World" Android application demonstrating project creation,
Android Studio interface, Android components, AVD creation, and application execution.

â† Back to Index

        Practical 01

Develop a simple "Hello World" Android application demonstrating project creation, Android
Studio interface, Android components, AVD creation, and application execution.

Project 1: Hello World

Project Name: HelloWorld

Template: Empty Views Activity

Project Architecture:

Total 5 files

I

Filename: MainActivity.java

package com.example.helloworld;

    import android.os.Bundle;
    import androidx.appcompat.app.AppCompatActivity;

    public class MainActivity extends AppCompatActivity {
         @Override
         protected void onCreate(Bundle savedInstanceState) {
             super.onCreate(savedInstanceState);
         setContentView(R.layout.activity_main);
         }
    }

================== PAGE BREAK ==================

PAGE 6
Path: app>java>com.example.helloworld>MainActivity.java

II

Filename: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

        xmlns:android="http://schemas.android.com/apk/res/android"

        android:layout_width="match_parent"

        android:layout_height="match_parent"

        android:orientation="vertical"

        android:gravity="center"

        android:padding="16dp">

        <TextView

        android:id="@+id/text_hello"

        android:layout_width="wrap_content"

        android:layout_height="wrap_content"

        android:text="Hello, World!"

        android:textSize="24sp"

        android:textStyle="bold"

================== PAGE BREAK ==================

PAGE 7
       android:textColor="#000000" />

</LinearLayout>

Path: app>res>layout>activity_main.xml

III

Filename: AndroidManifest.xml

<manifest xmlns:android="http://schemas.android.com/apk/res/android"
     package="com.example.helloworld">
     <application
    android:allowBackup="true"
     android:icon="@mipmap/ic_launcher"
     android:label="@string/app_name"
     android:roundIcon="@mipmap/ic_launcher_round"
     android:supportsRtl="true"
     android:theme="@style/Theme.Helloworld">
     <activity android:name=".MainActivity"
     android:exported="true"> <!-- Added android:exported attribute -->
     <intent-filter>
             <action android:name="android.intent.action.MAIN" />
      <category android:name="android.intent.category.LAUNCHER" />
     </intent-filter>

      </activity>
      </application>
</manifest>

Path: app>manifest>AndroidManifest.xml

================== PAGE BREAK ==================

PAGE 8
IV

Filename: colors.xml

<?xml version="1.0" encoding="utf-8"?>
 <resources>
      <color name="black">#FF000000</color>
      <color name="white">#FFFFFFFF</color>
      <color name="purple_500">#6200EE</color>
      <color name="purple_700">#3700B3</color>
 </resources>

Path: app>res>values>colors.xml

V

Filename: styles.xml

<?xml version="1.0" encoding="utf-8"?>
 <resources>
      <style name="Theme.Helloworld"
parent="Theme.MaterialComponents.DayNight.DarkActionBar">
      <!-- Customize your theme here -->
      <item name="colorPrimary">@color/purple_500</item>
      <item name="colorPrimaryVariant">@color/purple_700</item>
      <item name="colorOnPrimary">@color/white</item>
      </style>
 </resources>

Path: app>res>values>styles.xml

VI (Prebuild Project Code: To ensure proper project detail: No need to update until needed)

================== PAGE BREAK ==================

PAGE 9
Filename: build.gradle.kts (Module:app)

plugins {
       alias(libs.plugins.android.application)
  }

  android {
       namespace = "com.example.helloworld"
       compileSdk = 35

        defaultConfig {
        applicationId = "com.example.helloworld"
        minSdk = 24
        targetSdk = 35
        versionCode = 1
        versionName = "1.0"

        testInstrumentationRunner = "androidx.test.runner.AndroidJUnitRunner"
        }

        buildTypes {
        release {
             isMinifyEnabled = false
             proguardFiles(
        getDefaultProguardFile("proguard-android-optimize.txt"),
        "proguard-rules.pro"
             )
        }

           }
           compileOptions {
           sourceCompatibility = JavaVersion.VERSION_11
           targetCompatibility = JavaVersion.VERSION_11
           }
    }

    dependencies {

         implementation(libs.appcompat)
         implementation(libs.material)
         implementation(libs.activity)
         implementation(libs.constraintlayout)
         testImplementation(libs.junit)
         androidTestImplementation(libs.ext.junit)
         androidTestImplementation(libs.espresso.core)
    }

================== PAGE BREAK ==================

PAGE 10
Path: Gradle Scripts > build.gradle.kts

Above the Android Studio near Main Menu Click the Play button to Run the Program

Recommended compulsory AVD Emulator: Pixel 4 API 25 with version 7.1.1 Nougat

Output:

================== PAGE BREAK ==================

PAGE 11
Module 1 â€“ Practical 2
Develop an Android application demonstrating the use of Programming Resources
(colors.xml, themes.xml, strings.xml, dimens.xml, drawable resources) and apply them in UI
components.

â† Back to Index

     b.Develop an Android application demonstrating the use of Programming Resources
(colors.xml, themes.xml, strings.xml, dimens.xml, drawable resources) and apply them in
UI components.

Programming Resources

Android Resources: (Color, Theme, String, Drawable, Dimension, Image)

Project Name: Practical 2R

Template: Empty Views Activity

Language: Java

Project Architecture: 1 AndroidManifest.xml file, 6 Java Files,1 image in drawable image
file 6 layout .xml files and 4 values .xml files: Total 18 files.

Filename: AndroidManifest.xml

<?xml version="1.0" encoding="utf-8"?>
  <manifest xmlns:android="http://schemas.android.com/apk/res/android"
       xmlns:tools="http://schemas.android.com/tools">
       <application
       android:allowBackup="true"
       android:dataExtractionRules="@xml/data_extraction_rules"
       android:fullBackupContent="@xml/backup_rules"
       android:icon="@mipmap/ic_launcher"
       android:label="@string/app_name"
       android:roundIcon="@mipmap/ic_launcher_round"
       android:supportsRtl="true"
       android:theme="@style/Theme.AppCompat.Light"
       tools:targetApi="31">

        <activity android:name=".ThemeActivity" android:label="Theme Demo" />
        <activity android:name=".StringActivity" android:label="String Demo" />
        <activity android:name=".DrawableActivity" android:label="Drawable Demo"
/>
        <activity android:name=".DimensionActivity" android:label="Dimension
Demo" />
        <activity android:name=".ColorActivity" android:label="Color Demo" />

================== PAGE BREAK ==================

PAGE 12
        <activity
             android:name=".MainActivity"
             android:exported="true"
             android:label="@string/app_name"
             android:theme="@style/Theme.AppCompat.Light">
             <intent-filter>
        <action android:name="android.intent.action.MAIN" />

        <category android:name="android.intent.category.LAUNCHER" />
           </intent-filter>
      </activity>
      </application>
 </manifest>

Path: app>manifests>AndroidManifest.xml

Total 6 .java files path

1.Filename: ColorActivity.java

package com.example.practical2r;

  import android.os.Bundle;
  import androidx.appcompat.app.AppCompatActivity;

  public class ColorActivity extends AppCompatActivity {
       @Override
       protected void onCreate(Bundle savedInstanceState) {
       super.onCreate(savedInstanceState);
       setContentView(R.layout.activity_color);
       }
  }

2.Filename: DimensionActivity.java

package com.example.practical2r;

  import android.os.Bundle;

================== PAGE BREAK ==================

PAGE 13
  import androidx.appcompat.app.AppCompatActivity;

  public class DimensionActivity extends AppCompatActivity {
       @Override
       protected void onCreate(Bundle savedInstanceState) {
       super.onCreate(savedInstanceState);
       setContentView(R.layout.activity_dimension);
       }
  }

3.Filename: DrawableActivity.java

package com.example.practical2r;

  import android.os.Bundle;
  import androidx.appcompat.app.AppCompatActivity;

  public class DrawableActivity extends AppCompatActivity {
       @Override
       protected void onCreate(Bundle savedInstanceState) {
       super.onCreate(savedInstanceState);
       setContentView(R.layout.activity_drawable);
       }
  }

4.Filename: MainActivity.java

package com.example.practical2r;

  import android.content.Intent;
  import android.os.Bundle;
  import android.view.View;
  import androidx.appcompat.app.AppCompatActivity;

  public class MainActivity extends AppCompatActivity {
       @Override
       protected void onCreate(Bundle savedInstanceState) {
       super.onCreate(savedInstanceState);
       setContentView(R.layout.activity_main);
       }
       public void openColorActivity(View view) {
       startActivity(new Intent(this, ColorActivity.class));
       }
       public void openThemeActivity(View view) {
       startActivity(new Intent(this, ThemeActivity.class));
       }
       public void openStringActivity(View view) {

================== PAGE BREAK ==================

PAGE 14
       startActivity(new Intent(this, StringActivity.class));
       }
       public void openDrawableActivity(View view) {
       startActivity(new Intent(this, DrawableActivity.class));
       }
       public void openDimensionActivity(View view) {
       startActivity(new Intent(this, DimensionActivity.class));
       }
  }

5.Filename: StringActivity.java

package com.example.practical2r;

  import android.os.Bundle;
  import androidx.appcompat.app.AppCompatActivity;

  public class StringActivity extends AppCompatActivity {
       @Override
       protected void onCreate(Bundle savedInstanceState) {
       super.onCreate(savedInstanceState);
       setContentView(R.layout.activity_string);
       }
 }

6.Filename: ThemeActivity.java

package com.example.practical2r;

  import android.os.Bundle;
  import androidx.appcompat.app.AppCompatActivity;

  public class ThemeActivity extends AppCompatActivity {
       @Override
       protected void onCreate(Bundle savedInstanceState) {
       super.onCreate(savedInstanceState);
       setContentView(R.layout.activity_theme);
       }
 }

Image File Path

Image Detail: pebbles.jpg

================== PAGE BREAK ==================

PAGE 15
(Copy your image file from your local folder and only copy and paste into drawable folder.
Donâ€™t Drag and Drop). Image size must within KB size

Total 6 Layout .xml files path

1.Filename: activity_color.xml

<?xml version="1.0" encoding="utf-8"?>
 <RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
      android:layout_width="match_parent"
      android:layout_height="match_parent"
      android:background="@color/colorRed">
      <TextView
      android:layout_width="wrap_content"
      android:layout_height="wrap_content"
      android:text="Color Activity"
      android:textSize="24sp"
          android:layout_centerInParent="true"
      android:textColor="@color/white"/>
 </RelativeLayout>

2.Filename: activity_dimension.xml

<?xml version="1.0" encoding="utf-8"?>
 <LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
      android:layout_width="match_parent"
      android:layout_height="match_parent"
      android:orientation="vertical"
      android:padding="16dp"
      android:gravity="center">
      <TextView
      android:layout_width="wrap_content"
      android:layout_height="wrap_content"
      android:text="Dimension Activity"
      android:textSize="24sp"

      android:textColor="@android:color/black"/>
      <!-- Button demonstrating dimension usage -->
      <Button
          android:id="@+id/dimensionButton"
      android:layout_width="wrap_content"
      android:layout_height="wrap_content"
      android:text="Click Me!"
      android:textSize="@dimen/button_text_size"

================== PAGE BREAK ==================

PAGE 16
      android:padding="@dimen/button_padding"
      android:layout_marginTop="@dimen/button_margin_top"
      android:background="@color/btn_color"/>
 </LinearLayout>

3.Filename: activity_drawable.xml

<?xml version="1.0" encoding="utf-8"?>
 <RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
      android:layout_width="match_parent"
      android:layout_height="match_parent"
      android:background="@drawable/pebbles">
      <TextView
      android:layout_width="wrap_content"
      android:layout_height="wrap_content"
      android:text="Drawable Activity"
      android:textSize="24sp"
      android:layout_centerInParent="true"
      android:textColor="@android:color/white"/>
 </RelativeLayout>

4.Filename: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>
 <RelativeLayout
      xmlns:android="http://schemas.android.com/apk/res/android"
      xmlns:tools="http://schemas.android.com/tools"
      android:layout_width="match_parent"
      android:layout_height="match_parent"
      tools:context=".MainActivity"
      android:background="@drawable/pebbles">
      <Button
      android:id="@+id/btnColor"
      android:layout_width="wrap_content"
      android:layout_height="wrap_content"
      android:text="Color Demo"
      android:layout_centerHorizontal="true"
      android:layout_marginTop="50dp"
      android:onClick="openColorActivity"/>
      <Button
      android:id="@+id/btnTheme"

     android:layout_width="wrap_content"
     android:layout_height="wrap_content"
     android:text="Theme Demo"
     android:layout_below="@id/btnColor"
     android:layout_centerHorizontal="true"
     android:layout_marginTop="20dp"
     android:onClick="openThemeActivity"/>
     <Button
     android:id="@+id/btnString"
     android:layout_width="wrap_content"
     android:layout_height="wrap_content"
     android:text="String Demo"
     android:layout_below="@id/btnTheme"
     android:layout_centerHorizontal="true"
     android:layout_marginTop="20dp"
         android:onClick="openStringActivity"/>

================== PAGE BREAK ==================

PAGE 17
      <Button
     android:id="@+id/btnDrawable"
     android:layout_width="wrap_content"
     android:layout_height="wrap_content"
     android:text="Drawable Demo"
     android:layout_below="@id/btnString"
     android:layout_centerHorizontal="true"
     android:layout_marginTop="20dp"
     android:onClick="openDrawableActivity"/>
     <Button
     android:id="@+id/btnDimension"
     android:layout_width="wrap_content"
     android:layout_height="wrap_content"
     android:text="Dimension Demo"
     android:layout_below="@id/btnDrawable"
     android:layout_centerHorizontal="true"
     android:layout_marginTop="20dp"
     android:onClick="openDimensionActivity"/>
</RelativeLayout>

5.Filename: activity_string.xml

<?xml version="1.0" encoding="utf-8"?>
 <LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
      android:layout_width="match_parent"
      android:layout_height="match_parent"
      android:orientation="vertical"
      android:gravity="center"
      android:background="@color/colorPrimaryDark">
      <TextView
      android:layout_width="wrap_content"
      android:layout_height="wrap_content"
      android:text="@string/Welcome_Message"
      android:textSize="24sp"
      android:textColor="@android:color/white"/>
 </LinearLayout>

6.Filename: activity_theme.xml

<?xml version="1.0" encoding="utf-8"?>
 <RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
      android:layout_width="match_parent"
      android:layout_height="match_parent"
      android:background="@android:color/holo_blue_bright">
      <TextView
      android:layout_width="wrap_content"
      android:layout_height="wrap_content"
      android:text="You got this sky blue theme"
      android:textSize="24sp"
      android:layout_centerInParent="true"
      android:textColor="@android:color/black"/>
 </RelativeLayout>

================== PAGE BREAK ==================

PAGE 18
Total 4 values .xml files

1.Filename: colors.xml

<?xml version="1.0" encoding="utf-8"?>
 <resources>
     <color name="purple_200">#FFBB86FC</color>
     <color name="purple_500">#FF6200EE</color>
     <color name="purple_700">#FF3700B3</color>
     <color name="teal_200">#9ADA03</color>
     <color name="teal_700">#FF018786</color>
     <color name="black">#FF000000</color>
     <color name="white">#FFFFFFFF</color>
     <color name="btn_color">#FFC49662</color>
     <color name="colorRed">#E91E63</color>
     <color name="colorBlue">#0000FF</color>
     <color name="colorPrimary">#6200EE</color>
     <color name="colorPrimaryDark">#3700B3</color>
     <color name="colorAccent">#03DAC5</color>
 </resources>

2.Filename: dimens.xml

<?xml version="1.0" encoding="utf-8"?>
 <resources>
     <dimen name="button_margin_top">24dp</dimen>
     <dimen name="button_padding">16dp</dimen>
     <dimen name="button_text_size">18sp</dimen>
 </resources>

3.Filename: strings.xml

<resources>
     <string name="app_name">Practical 2R</string>
     <string name="button_name">Click on me</string>
     <string name="ParaHead">Welcome to Practical 2R</string>
     <string name="Description">This is a string resource demo.</string>

================== PAGE BREAK ==================

PAGE 19
     <string name="Welcome_Message">Welcome to Android Studio. This is your
Practical 2 Resources.</string>
 </resources>

4.Filename: themes.xml

<?xml version="1.0" encoding="utf-8"?>
 <resources>
      <style name="AppTheme" parent="Theme.AppCompat.Light.DarkActionBar">
        <item name="colorPrimary">@color/colorPrimary</item>
      <item name="colorPrimaryDark">@color/colorPrimaryDark</item>
      <item name="colorAccent">@color/colorAccent</item>
      </style>
      <style name="BlueTheme" parent="Theme.AppCompat.Light.DarkActionBar">
      <item name="colorPrimary">@color/colorPrimary</item>
      <item name="colorPrimaryDark">@color/colorPrimaryDark</item>
      <item name="colorAccent">@color/colorAccent</item>
      <item name="android:background">#00F0EF</item>
      <item name="android:textColor">#000000</item>
      </style>
 </resources>

Above the Android Studio near Main Menu Click the Play button to Run the Program

Recommended compulsory AVD Emulator: Pixel 4 API 25 with version 7.1.1 Nougat

Play Emulator

Output:

MAIN PAGE

Click COLOR DEMO press back & Click THEME DEMO press back & Click THEME DEMO

================== PAGE BREAK ==================

PAGE 20
Press back & Click COLOR DEMO Press back & Click COLOR DEMO

================== PAGE BREAK ==================

PAGE 21
Module 1 â€“ Practical 3
Develop an Android application demonstrating complete Activity Lifecycle methods and
analyze execution using Logcat.

â† Back to Index

C. Develop an Android application demonstrating complete Activity Lifecycle methods
and analyze execution using Logcat.

Project Name: logcat

package com.example.logact;

import android.os.Bundle;
import android.util.Log;

import androidx.activity.EdgeToEdge;
import androidx.appcompat.app.AppCompatActivity;
import androidx.core.graphics.Insets;
import androidx.core.view.ViewCompat;
import androidx.core.view.WindowInsetsCompat;

public class MainActivity extends AppCompatActivity {

   @Override
   protected void onCreate(Bundle savedInstanceState) {
       super.onCreate(savedInstanceState);
       setContentView(R.layout.activity_main);
   }

   @Override
   protected void onStart() {
       super.onStart();
       Log.d("on start invoked", "on started");

   }

   @Override
   protected void onPostResume() {
       super.onPostResume();

================== PAGE BREAK ==================

PAGE 22
        Log.d("on resume invoked", "on resume");
    }

    @Override
    protected void onPause() {
        super.onPause();
        Log.d("on pause invoked", "on pause");
    }

    @Override
        protected void onStop() {

            super.onStop();
            Log.d("on stop invoked", "on stopped");
        }

    @Override
    protected void onDestroy() {
        super.onDestroy();
        Log.d("on destroy invoked", "on destroy");
    }
}

================== PAGE BREAK ==================

PAGE 23
Module 1 â€“ Practical 4
Develop an Android application to create and integrate a Fragment and demonstrate
Fragment lifecycle methods.

â† Back to Index

        2. Fragments and Activity Interaction

4. Develop an Android application to create and integrate a Fragment and demonstrate
Fragment lifecycle methods.

Project Name: FragmentLifecycleDemo

Create a new fragment class:

java->new-> fragment->fragment(blank)

Fragment Name: DemoFragment

Fragment Layout name: fragment_demo

I

Filename: DemoFragment.java

package com.example.fragmentlifecycledemo;

import android.content.Context;

import android.os.Bundle;

import android.util.Log;

import android.view.LayoutInflater; import android.view.View;

import android.view.ViewGroup;

import androidx.annotation.NonNull; import androidx.annotation.Nullable;

================== PAGE BREAK ==================

PAGE 24
import androidx.fragment.app.Fragment;

public class DemoFragment extends Fragment {

   String TAG = "FragmentLifecycle";

   @Override

   public void onAttach(@NonNull Context context) {

   super.onAttach(context);

   Log.d(TAG, "onAttach() executed");}

   @Override

   public void onCreate(Bundle savedInstanceState) {

       super.onCreate(savedInstanceState);

       Log.d(TAG, "onCreate() executed");

   }

   @Override

  public View onCreateView(LayoutInflater inflater, ViewGroup

================== PAGE BREAK ==================

PAGE 25
container,Bundle savedInstanceState) {

        Log.d(TAG, "onCreateView() executed");

        return inflater.inflate(R.layout.fragment_demo, container, false);

    }

@Override

public void onViewCreated(@NonNull View view, @Nullable Bundle
savedInstanceState) {

        super.onViewCreated(view, savedInstanceState);

         Log.d("on view created invoked", "onViewCreated() executed");

}

    @Override

    public void onStart() {

        super.onStart();

        Log.d("on start invoked", "on started");

}

================== PAGE BREAK ==================

PAGE 26
@Override

public void onResume() {

    super.onResume();

    Log.d("on resume invoked", "on resume");

}

@Override

public void onPause() {

    super.onPause();

    Log.d("on pause invoked", "on pause");

}

@Override

public void onStop() {

    super.onStop();

    Log.d("on stop invoked", "on stopped");

}

================== PAGE BREAK ==================

PAGE 27
@Override

public void onDestroyView() {

    super.onDestroyView();

    Log.d("on destroyview invoked", "on destroyview() executed");

}

    @Override

    public void onDestroy() {

        super.onDestroy();

        Log.d("on destroy invoked", "on destroy");

    }

    @Override

    public void onDetach() {

        super.onDetach();

        Log.d("on detach invoked", "on detach");

    }

}

================== PAGE BREAK ==================

PAGE 28
Filename: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>

<androidx.constraintlayout.widget.ConstraintLayout
xmlns:android="http://schemas.android.com/apk/res/android"

    xmlns:app="http://schemas.android.com/apk/res-auto"

    xmlns:tools="http://schemas.android.com/tools"

    android:id="@+id/fragment_container_view_tag"

    android:layout_width="match_parent"

    android:layout_height="match_parent"

    tools:context=".MainActivity">

    <TextView

       android:layout_width="wrap_content"

       android:layout_height="wrap_content"

       android:text="Hello World!"

       app:layout_constraintBottom_toBottomOf="parent"

       app:layout_constraintEnd_toEndOf="parent"

       app:layout_constraintStart_toStartOf="parent"

       app:layout_constraintTop_toTopOf="parent" />

================== PAGE BREAK ==================

PAGE 29
</androidx.constraintlayout.widget.ConstraintLayout>

Filename: MainActivity.java

package com.example.fragmentlifecycledemo;

import android.os.Bundle;

import androidx.fragment.app.FragmentTransaction;

import androidx.activity.EdgeToEdge;

import androidx.appcompat.app.AppCompatActivity;

import androidx.core.graphics.Insets;

import androidx.core.view.ViewCompat;

import androidx.core.view.WindowInsetsCompat;

public class MainActivity extends AppCompatActivity {

================== PAGE BREAK ==================

PAGE 30
   @Override

   protected void onCreate(Bundle savedInstanceState) {

       super.onCreate(savedInstanceState);

      setContentView(R.layout.activity_main);

        DemoFragment fragment = new DemoFragment();

        FragmentTransaction transaction =

        getSupportFragmentManager().beginTransaction();

        transaction.replace(R.id.fragment_container_view_tag,
fragment);

        transaction.commit();

      }

  }

fragment_demo.xml

<?xml version="1.0" encoding="utf-8"?>

<FrameLayout xmlns:android="http://schemas.android.com/apk/res/android"

 xmlns:tools="http://schemas.android.com/tools"

  android:layout_width="match_parent"

================== PAGE BREAK ==================

PAGE 31
 android:layout_height="match_parent"

 tools:context=".DemoFragment">

 <!-- TODO: Update blank fragment layout -->

 <TextView

      android:layout_width="match_parent"

      android:layout_height="match_parent"

      android:text="@string/hello_blank_fragment" />

</FrameLayout>

================== PAGE BREAK ==================

PAGE 32
Module 1 â€“ Practical 5
Develop an Android application implementing Fragment-based UI navigation between
multiple screens.

â† Back to Index

5. Develop an Android application implementing Fragment-based UI navigation between
multiple screens.

Activity Life Cycle, Activity methods, Multiple Activities, Life Cycle of fragments and
multiple fragments.

Project Name: Fragment Lifecycle

Template: Empty Views Activity

Language: Java

Project Architecture: Total 6 files

I Filename: MainActivity.java

package com.example.fragmentlifecycle;

  import androidx.appcompat.app.AppCompatActivity;
  import android.os.Bundle;
  import android.widget.Button;

  public class MainActivity extends AppCompatActivity {

        private boolean isFragmentOneLoaded = true;
        private final androidx.fragment.app.FragmentManager fragmentManager =
getSupportFragmentManager();

        @Override
        protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

           Button btnChange = findViewById(R.id.btn_change); // Ensure ID
matches activity_main.xml
        loadFragmentOne();

================== PAGE BREAK ==================

PAGE 33
       btnChange.setOnClickListener(v -> {
             if (isFragmentOneLoaded) {
        loadFragmentTwo();
             } else {
        loadFragmentOne();
             }
       });
       }

       private void loadFragmentOne() {
            androidx.fragment.app.FragmentTransaction transaction =
fragmentManager.beginTransaction();
       FragmentOne fragment = new FragmentOne();
       transaction.replace(R.id.fragment_holder, fragment); // Ensure ID
matches activity_main.xml
       transaction.addToBackStack(null);
       transaction.commit();
       isFragmentOneLoaded = true;
       }

       private void loadFragmentTwo() {
            androidx.fragment.app.FragmentTransaction transaction =
fragmentManager.beginTransaction();
       FragmentTwo fragment = new FragmentTwo();
       transaction.replace(R.id.fragment_holder, fragment); // Ensure ID
matches activity_main.xml

      transaction.addToBackStack(null);
      transaction.commit();
      isFragmentOneLoaded = false;
      }
 }

Path: app>java>com.example.fragmentlifecycle>MainActivity.java

II

Filename: FragmentOne.java

package com.example.fragmentlifecycle;

================== PAGE BREAK ==================

PAGE 34
import android.content.Context;
import android.os.Bundle;
import android.util.Log;
import android.view.LayoutInflater;
import android.view.View;
import android.view.ViewGroup;
import androidx.fragment.app.Fragment;
public class FragmentOne extends Fragment {
      private static final String TAG = "FragmentOne";
      @Override
      public void onAttach(Context context) {
      super.onAttach(context);

          Log.d(TAG, "onAttach");
          }
          @Override
          public View onCreateView(LayoutInflater inflater, ViewGroup container, Bundle
savedInstanceState) {
          Log.d(TAG, "onCreateView");
          return inflater.inflate(R.layout.fragment_one, container, false);
          }

}

Path: app>java>com.example.fragmentlifecycle > FragmentOne.java

III

Filename: FragmentTwo.java

package com.example.fragmentlifecycle;
import android.content.Context;
import android.os.Bundle;
import android.util.Log;
import android.view.LayoutInflater;
import android.view.View;
import android.view.ViewGroup;
import androidx.fragment.app.Fragment;
public class FragmentTwo extends Fragment {
      private static final String TAG = "FragmentTwo";

           @Override
           public void onAttach(Context context) {
           super.onAttach(context);
          Log.d(TAG, "onAttach");
      }
          @Override

================== PAGE BREAK ==================

PAGE 35
     public View onCreateView(LayoutInflater inflater, ViewGroup container, Bundle
savedInstanceState) {
     Log.d(TAG, "onCreateView");
     return inflater.inflate(R.layout.fragment_two, container, false);
     }
}

Path: app>java>com.example.fragmentlifecycle > FragmentTwo.java

IV

Filename: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
  android:layout_width="match_parent"
  android:layout_height="match_parent"
  android:orientation="vertical">
  <Button
     android:id="@+id/btn_change"
     android:layout_width="match_parent"

     android:layout_height="wrap_content"
     android:text="Change Fragment" />
  <FrameLayout
     android:id="@+id/fragment_holder"
     android:layout_width="match_parent"
     android:layout_height="0dp"
     android:layout_weight="1" />
</LinearLayout>
Path: app>res>layout>activity_main.xml

V

Filename: fragment_one.xml

<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
      android:layout_width="match_parent"
      android:layout_height="match_parent">
      <TextView
      android:id="@+id/textView"

================== PAGE BREAK ==================

PAGE 36
      android:layout_width="wrap_content"
      android:layout_height="wrap_content"
      android:layout_centerInParent="true"
      android:text="Fragment One"
      android:textSize="24sp" />
</RelativeLayout>

Path: app>res>layout>fragment_one.xml

VI

Filename: fragment_two.xml

<?xml version="1.0" encoding="utf-8"?>

<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
         android:layout_width="match_parent"
         android:layout_height="match_parent">
         <TextView
         android:id="@+id/textView2"
         android:layout_width="wrap_content"
         android:layout_height="wrap_content"
         android:layout_centerInParent="true"
         android:text="Fragment Two"
         android:textSize="24sp" />
</RelativeLayout>

Path: app>res>layout>fragment_two.xml

Above the Android Studio near Main Menu Click the Play button to Run the Program

================== PAGE BREAK ==================

PAGE 37
Module 1 â€“ Practical 6
Develop an Android application demonstrating communication between Activity and
Fragment.

â† Back to Index

6. Develop an Android application demonstrating communication between Activity and
Fragment.

Project Name: ActivityFragmentCommunication

Creating Fragment
java package â†’ Newâ†’ Fragment â†’ Fragment (Blank)
Fragment Name: DemoFragment
Layout Name: fragment_demo

Filename: activity_main.xml
<?xml version="1.0" encoding="utf-8"?>

<FrameLayout

    xmlns:android="http://schemas.android.com/apk/res/android"

    android:id="@+id/fragment_container"

    android:layout_width="match_parent"

    android:layout_height="match_parent"/>

Open From res/layout:
Filename: fragment_demo.xml
<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

================== PAGE BREAK ==================

PAGE 38
   xmlns:android="http://schemas.android.com/apk/res/android"

   android:layout_width="match_parent"

   android:layout_height="match_parent"

   android:gravity="center"

   android:orientation="vertical"

   android:padding="20dp">

   <TextView

      android:id="@+id/txtMessage"

       android:layout_width="wrap_content" android:layout_height="wrap_content"
android:textSize="22sp"

      android:text="Message from Activity"/>

   <Button

      android:id="@+id/btnSend"

      android:layout_width="wrap_content"

      android:layout_height="wrap_content"

      android:text="Send Message to Activity"

      android:layout_marginTop="20dp"/>

================== PAGE BREAK ==================

PAGE 39
</LinearLayout>

Modify DemoFragment.java.
Filename: DemoFragment.java

package com.example.activityfragmentcommunication;

import android.content.Context;

import android.os.Bundle;

import android.view.LayoutInflater;

import android.view.View;

import android.view.ViewGroup; import android.widget.Button;

import android.widget.TextView;

import androidx.annotation.NonNull;

import androidx.annotation.Nullable;

import androidx.fragment.app.Fragment;

public class DemoFragment extends Fragment

{

    TextView txtMessage;

================== PAGE BREAK ==================

PAGE 40
    Button btnSend;

    String activityMessage;

    FragmentCommunication communication;

public interface FragmentCommunication {

    void onMessageFromFragment(String message);

}

// Receive Activity object

@Override

public void onAttach(@NonNull Context context) {

    super.onAttach(context);

    communication = (FragmentCommunication) context;

}

// Method to receive data from Activity

================== PAGE BREAK ==================

PAGE 41
public static DemoFragment newInstance(String message) {

    DemoFragment fragment = new DemoFragment();

    Bundle bundle = new Bundle();

    bundle.putString("msg", message);

    fragment.setArguments(bundle);

    return fragment;

}

@Override

public View onCreateView(LayoutInflater inflater,ViewGroup container,Bundle
savedInstanceState) {

    View view = inflater.inflate(R.layout.fragment_demo,container, false);

    txtMessage = view.findViewById(R.id.txtMessage);

    btnSend = view.findViewById(R.id.btnSend);

// Receiving data from Activity

    if(getArguments() != null){

         activityMessage = getArguments().getString("msg");

         txtMessage.setText(activityMessage);

    }

================== PAGE BREAK ==================

PAGE 42
// Sending data to Activity

    btnSend.setOnClickListener(v -> {

          communication.onMessageFromFragment(

        "Hello Activity! Message from Fragment");

    }

    );

          return view;

}

}

Filename: MainActivity.java

package com.example.activityfragmentcommunication;

import android.os.Bundle;

import android.widget.Toast;

================== PAGE BREAK ==================

PAGE 43
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity

      implements DemoFragment.FragmentCommunication {

   @Override

   protected void onCreate(Bundle savedInstanceState) {

      super.onCreate(savedInstanceState);

      setContentView(R.layout.activity_main);

      // Sending data from Activity to Fragment

      DemoFragment fragment = DemoFragment.newInstance(

               "Hello Fragment! Message from Activity"

       );

================== PAGE BREAK ==================

PAGE 44
        getSupportFragmentManager()

                .beginTransaction()

                .replace(R.id.fragment_container, fragment)

                .commit();

    }

    // Receiving data from Fragment

    @Override

    public void onMessageFromFragment(String message) {

        Toast.makeText(this, message, Toast.LENGTH_LONG).show();

    }

}

OUTPUT:

================== PAGE BREAK ==================

PAGE 45
Module 1 â€“ Practical 7
Develop an Android application using LinearLayout (Horizontal and Vertical) to design
structured UI.

â† Back to Index

        III. Basic Layout Management

7. Develop an Android application using LinearLayout (Horizontal and Vertical) to design
structured UI.

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

 xmlns:android="http://schemas.android.com/apk/res/android"

   android:id="@+id/main"

   android:layout_width="match_parent"

   android:layout_height="match_parent"

   android:orientation="vertical"

   android:padding="20dp">

   <!-- Title -->

   <TextView

       android:layout_width="wrap_content"

       android:layout_height="wrap_content"

       android:text="Student Registration" android:textSize="26sp"

       android:textStyle="bold"

       android:layout_gravity="center" android:layout_marginBottom="20dp"/>

================== PAGE BREAK ==================

PAGE 46
  <!--Vertical Layout Components -->

  <EditText

       android:id="@+id/etName"

       android:layout_width="match_parent"

       android:layout_height="wrap_content"

       android:hint="Enter Name"

       android:layout_marginBottom="10dp"/>

<EditText

  android:id="@+id/etEmail"

  android:layout_width="match_parent"

  android:layout_height="wrap_content"

  android:hint="Enter Email"

  android:layout_marginBottom="20dp"/>

<!-- Horizontal LinearLayout -->

<LinearLayout

  android:layout_width="match_parent"

  android:layout_height="wrap_content"

  android:orientation="horizontal"

================== PAGE BREAK ==================

PAGE 47
  android:gravity="center">

  <Button

      android:id="@+id/btnSubmit"

      android:layout_width="wrap_content"

      android:layout_height="wrap_content"

      android:text="Submit"/>

  <Button

      android:id="@+id/btnReset"

      android:layout_width="wrap_content"

      android:layout_height="wrap_content"

      android:text="Reset"

      android:layout_marginStart="20dp"/>

</LinearLayout>

</LinearLayout>

================== PAGE BREAK ==================

PAGE 48
Module 1 â€“ Practical 8
Develop an Android application using RelativeLayout to align UI components dynamically.

â† Back to Index

b) Develop an Android application using RelativeLayout to align UI components dynamically.

Project Name: RelativeLayout

I Filename: activity_main.xml
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
   xmlns:tools="http://schemas.android.com/tools"
   android:id="@+id/main"
   android:layout_width="match_parent"
   android:layout_height="match_parent"
   android:padding="16dp"
   tools:context=".MainActivity">
   <TextView
      android:id="@+id/title"
      android:layout_width="wrap_content"
      android:layout_height="wrap_content"
      android:layout_centerHorizontal="true"
      android:text="RelativeLayout Demo"
      android:textSize="28sp"
      android:textStyle="bold" />
   <ImageView
      android:id="@+id/star"
      android:layout_width="100dp"
      android:layout_height="100dp"
      android:layout_below="@id/title"
      android:layout_centerHorizontal="true"
      android:layout_marginTop="24dp"
      android:contentDescription="Star image"
      android:src="@android:drawable/btn_star_big_on" />
   <EditText
      android:id="@+id/etName"
      android:layout_width="match_parent"
      android:layout_height="wrap_content"
      android:layout_below="@id/star"
      android:layout_marginTop="24dp"
      android:hint="Enter Name"
      android:inputType="textPersonName" />
   <Button
      android:id="@+id/btnSubmit"
      android:layout_width="wrap_content"
      android:layout_height="wrap_content"
      android:layout_below="@id/etName"
      android:layout_alignParentStart="true"
      android:layout_marginTop="20dp"
      android:text="SUBMIT" />
   <Button
      android:id="@+id/btnReset"

================== PAGE BREAK ==================

PAGE 49
      android:layout_width="wrap_content"
      android:layout_height="wrap_content"
      android:layout_below="@id/etName"
      android:layout_alignParentEnd="true"
      android:layout_marginTop="20dp"
      android:text="RESET" />
</RelativeLayout>
II Filename: main_activity.java

package com.example.relativelayoutdemo;

import android.os.Bundle;
import android.widget.Button;
import android.widget.EditText;
import android.widget.Toast;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    @Override

    protected void onCreate(Bundle savedInstanceState) {

        super.onCreate(savedInstanceState);

        setContentView(R.layout.activity_main);

        EditText etName = findViewById(R.id.etName);

        Button btnSubmit = findViewById(R.id.btnSubmit);

        Button btnReset = findViewById(R.id.btnReset);

        btnSubmit.setOnClickListener(v -> {

              String name = etName.getText().toString().trim();

              if (name.isEmpty()) {

        Toast.makeText(this, "Enter your name", Toast.LENGTH_SHORT).show();

              } else {

        Toast.makeText(this, "Hello, " + name, Toast.LENGTH_SHORT).show();

              }

        });

        btnReset.setOnClickListener(v -> etName.setText(""));

    }

}

================== PAGE BREAK ==================

PAGE 50
Module 1 â€“ Practical 9
Develop an Android application using TableLayout to design a structured
Login/Registration Form.

â† Back to Index

c) Develop an Android application using TableLayout to design a structured Login/Registration Form.

Project Name: TableLayout

I Filename: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
  android:id="@+id/main"
 xmlns:android="http://schemas.android.com/apk/res/android"
 xmlns:app="http://schemas.android.com/apk/res-auto"
 xmlns:tools="http://schemas.android.com/tools"
  android:layout_width="match_parent"
  android:layout_height="match_parent">

  <TableLayout
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:layout_margin="16dp"
    app:layout_constraintTop_toTopOf="parent"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintEnd_toEndOf="parent"
    android:stretchColumns="1">

    <!-- Heading -->
    <TableRow>

      <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_span="2"
        android:gravity="center"
        android:text="Student Registration"
        android:textSize="28sp"
        android:textStyle="bold"
        android:padding="16dp"/>
    </TableRow>

    <!-- Name -->
    <TableRow>

       <TextView
         android:layout_width="wrap_content"
         android:layout_height="wrap_content"

        android:text="Name"
        android:textSize="18sp"

================== PAGE BREAK ==================

PAGE 51
    android:padding="8dp"/>

  <EditText
    android:id="@+id/etName"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:hint="Enter Name"
    android:inputType="textPersonName"/>
</TableRow>

<!-- Email -->
<TableRow>

  <TextView
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Email"
    android:textSize="18sp"
    android:padding="8dp"/>

  <EditText
    android:id="@+id/etEmail"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:hint="Enter Email"
    android:inputType="textEmailAddress"/>
</TableRow>

<!-- Password -->
<TableRow>

  <TextView
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Password"
    android:textSize="18sp"
    android:padding="8dp"/>

  <EditText
    android:id="@+id/etPassword"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"

    android:hint="Enter Password"
    android:inputType="textPassword"/>
</TableRow>

<!-- Buttons -->
<TableRow
  android:gravity="center"
  android:paddingTop="20dp">

   <Button
     android:id="@+id/btnRegister"
     android:layout_width="wrap_content"
     android:layout_height="wrap_content"
     android:text="Register"/>

================== PAGE BREAK ==================

PAGE 52
       <Button
         android:id="@+id/btnReset"
         android:layout_width="wrap_content"
         android:layout_height="wrap_content"
         android:layout_marginStart="20dp"
         android:text="Reset"/>
    </TableRow>
  </TableLayout>
</androidx.constraintlayout.widget.ConstraintLayout>

II Filename: main_activity.java
package com.example.tabledemo;

import android.os.Bundle;
import android.widget.Button;
import android.widget.EditText;
import android.widget.Toast;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {
  private EditText etName, etEmail, etPassword;
  private Button btnRegister, btnReset;

  @Override
  protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);
    etName = findViewById(R.id.etName);
    etEmail = findViewById(R.id.etEmail);
    etPassword = findViewById(R.id.etPassword);

    btnRegister = findViewById(R.id.btnRegister);

    btnReset = findViewById(R.id.btnReset);

    btnRegister.setOnClickListener(v -> {

          String name = etName.getText().toString().trim();

          String email = etEmail.getText().toString().trim();

          String password = etPassword.getText().toString();

          if (name.isEmpty() || email.isEmpty() || password.isEmpty()) {

              Toast.makeText(this, "Please fill in all fields", Toast.LENGTH_SHORT).show();

          } else {

              Toast.makeText(this, "Registration submitted", Toast.LENGTH_SHORT).show();

          }

    });

    btnReset.setOnClickListener(v -> {

================== PAGE BREAK ==================

PAGE 53
              etName.setText("");

              etEmail.setText("");

              etPassword.setText("");

        });

    }

}

Module 1 â€“ Practical 10
Develop an Android application using ScrollView to display long scrollable content.

â† Back to Index

a) Develop an Android application using ScrollView to display long scrollable content.

Project Name: ScrollViewLayout

I Filename: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>
<ScrollView xmlns:android="http://schemas.android.com/apk/res/android"
  android:layout_width="match_parent"
  android:layout_height="match_parent"
  android:fillViewport="true">
  <LinearLayout
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:orientation="vertical"
    android:padding="16dp">
    <TextView
       android:layout_width="match_parent"
       android:layout_height="wrap_content"
       android:layout_marginBottom="20dp"
       android:gravity="center"
       android:text="Student Registration Form"
       android:textSize="24sp"
       android:textStyle="bold" />

================== PAGE BREAK ==================

PAGE 54
     <EditText android:id="@+id/etName" android:layout_width="match_parent"
android:layout_height="wrap_content" android:hint="Enter Full Name" android:inputType="textPersonName"
/>
     <EditText android:id="@+id/etEmail" android:layout_width="match_parent"
android:layout_height="wrap_content" android:hint="Enter Email" android:inputType="textEmailAddress" />
     <EditText android:id="@+id/etPhone" android:layout_width="match_parent"
android:layout_height="wrap_content" android:hint="Enter Phone Number" android:inputType="phone" />
     <EditText android:id="@+id/etAddress" android:layout_width="match_parent"
android:layout_height="wrap_content" android:hint="Enter Address" android:inputType="textPostalAddress"
/>
     <EditText android:id="@+id/etCity" android:layout_width="match_parent"
android:layout_height="wrap_content" android:hint="Enter City" android:inputType="textCapWords" />
     <EditText android:id="@+id/etState" android:layout_width="match_parent"
android:layout_height="wrap_content" android:hint="Enter State" android:inputType="textCapWords" />
     <EditText android:id="@+id/etCountry" android:layout_width="match_parent"
android:layout_height="wrap_content" android:hint="Enter Country" android:inputType="textCapWords" />
     <EditText android:id="@+id/etQualification" android:layout_width="match_parent"
android:layout_height="wrap_content" android:hint="Enter Qualification" android:inputType="textCapWords"
/>
     <EditText android:id="@+id/etSkills" android:layout_width="match_parent"
android:layout_height="wrap_content" android:hint="Enter Skills" android:inputType="textMultiLine" />
     <EditText android:id="@+id/etExperience" android:layout_width="match_parent"
android:layout_height="wrap_content" android:hint="Enter Experience" android:inputType="textMultiLine" />
     <EditText android:id="@+id/etCollege" android:layout_width="match_parent"
android:layout_height="wrap_content" android:hint="Enter College Name"
android:inputType="textCapWords" />
     <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:gravity="center"
        android:orientation="horizontal">
        <Button android:id="@+id/btnSubmit" android:layout_width="wrap_content"
android:layout_height="wrap_content" android:text="Submit" />
        <Button android:id="@+id/btnReset" android:layout_width="wrap_content"
android:layout_height="wrap_content" android:layout_marginStart="16dp" android:text="Reset" />
     </LinearLayout>
   </LinearLayout>
</ScrollView>

Module 1 â€“ Practical 11
Develop an Android application using AbsoluteLayout demonstrating fixed positioning.

â† Back to Index

b) Develop an Android application using AbsoluteLayout demonstrating fixed positioning.

Project Name : AbsoluteLayout

================== PAGE BREAK ==================

PAGE 55
I Filename: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>

<androidx.constraintlayout.widget.ConstraintLayout
xmlns:android="http://schemas.android.com/apk/res/android"

xmlns:app="http://schemas.android.com/apk/res-auto"

xmlns:tools="http://schemas.android.com/tools"

 android:id="@+id/main"

 android:layout_width="match_parent"

 android:layout_height="match_parent"

tools:context=".MainActivity">

 <AbsoluteLayout

   android:layout_width="408dp"

   android:layout_height="728dp"

   app:layout_constraintBottom_toBottomOf="parent"

   app:layout_constraintEnd_toEndOf="parent"

   app:layout_constraintHorizontal_bias="0.497"

   app:layout_constraintStart_toStartOf="parent"

   app:layout_constraintTop_toTopOf="parent"

   app:layout_constraintVertical_bias="0.139">

   <TextView

     android:id="@+id/textView"

     android:layout_width="275dp"

================== PAGE BREAK ==================

PAGE 56
 android:layout_height="54dp"

 android:layout_x="60dp"

 android:layout_y="30dp"

 android:text="Absolute Layout Demo"

 android:textAlignment="center"

 android:textSize="24sp"

 android:textStyle="bold" />

<TextView

 android:id="@+id/textView2"

 android:layout_width="87dp"

 android:layout_height="40dp"

 android:layout_x="30dp"

 android:layout_y="100dp"

 android:text="Name"

 android:textAlignment="center"

 android:textSize="20sp" />

<TextView

 android:id="@+id/textView3"

 android:layout_width="87dp"

 android:layout_height="40dp"

 android:layout_x="30dp"

 android:layout_y="170dp"

 android:text="Email"

================== PAGE BREAK ==================

PAGE 57
 android:textAlignment="center"

 android:textSize="20sp" />

<EditText

 android:id="@+id/editTextText"

 android:layout_width="wrap_content"

 android:layout_height="wrap_content"

 android:layout_x="100dp"

 android:layout_y="90dp"

 android:ems="10"

 android:inputType="text"

 android:text="Enter Name" />

<EditText

 android:id="@+id/editTextText1"

 android:layout_width="wrap_content"

 android:layout_height="wrap_content"

 android:layout_x="100dp"

 android:layout_y="160dp"

 android:ems="10"

 android:inputType="text"

 android:text="Enter Email" />

<Button

 android:id="@+id/button"

================== PAGE BREAK ==================

PAGE 58
    android:layout_width="wrap_content"

    android:layout_height="wrap_content"

    android:layout_x="50dp"

    android:layout_y="250dp"

    android:text="Submit" />

  <Button

    android:id="@+id/button2"

    android:layout_width="wrap_content"

    android:layout_height="wrap_content"

    android:layout_x="190dp"

    android:layout_y="250dp"

    android:text="Reset" />

</AbsoluteLayout>

</androidx.constraintlayout.widget.ConstraintLayout>

================== PAGE BREAK ==================

PAGE 59
Module 1 â€“ Practical 12
Develop an Android application using FrameLayout to overlay UI elements.

â† Back to Index

c) Develop an Android application using FrameLayout to overlay UI elements.

Project Name : FrameLayout

I Filename: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>
<FrameLayout xmlns:android="http://schemas.android.com/apk/res/android"
  xmlns:tools="http://schemas.android.com/tools"
  android:id="@+id/main"
  android:layout_width="match_parent"
  android:layout_height="match_parent"
  tools:context=".MainActivity">
  <ImageView
     android:layout_width="match_parent"
     android:layout_height="match_parent"
     android:contentDescription="Background star"
     android:scaleType="centerInside"
     android:src="@android:drawable/btn_star_big_on" />
  <TextView
     android:layout_width="match_parent"
     android:layout_height="wrap_content"
     android:layout_gravity="center"
     android:gravity="center"
     android:text="Welcome to FrameLayout"
     android:textSize="24sp"
     android:textStyle="bold" />
  <Button
     android:id="@+id/button"
     android:layout_width="wrap_content"
     android:layout_height="wrap_content"
     android:layout_gravity="bottom|center_horizontal"
     android:layout_marginBottom="24dp"
     android:text="Click here" />
</FrameLayout>

II Filename: main_activity.java

package com.example.framelayout;

================== PAGE BREAK ==================

PAGE 60
import android.os.Bundle;
import android.widget.Button;
import android.widget.Toast;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {
  @Override
  protected void onCreate(Bundle savedInstanceState) {
     super.onCreate(savedInstanceState);
     setContentView(R.layout.activity_main);
     Button button = findViewById(R.id.button);
     button.setOnClickListener(v -> Toast.makeText(this, "Button clicked",
Toast.LENGTH_SHORT).show());
  }
}

Module 1 â€“ Practical 13
Develop an Android application using ListView with ArrayAdapter and implement item click
handling.

â† Back to Index

a) Develop an Android application using ListView with ArrayAdapter and implement
item click handling.

Project Name: ListViewDemo

I Filename: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>
<LinearLayout
 xmlns:android="http://schemas.android.com/apk/res/android"
  android:id="@+id/main"
  android:layout_width="match_parent"
  android:layout_height="match_parent"
  android:orientation="vertical"
  android:padding="10dp">

  <TextView
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Programming Languages"
    android:textSize="24sp"
    android:textStyle="bold"
    android:paddingBottom="10dp" />

================== PAGE BREAK ==================

PAGE 61
  <ListView
    android:id="@+id/listView"
    android:layout_width="match_parent"
    android:layout_height="match_parent" />
</LinearLayout>

II Filename: main_activity.java

package com.example.listviewdemo;
import android.os.Bundle;
import android.view.View;
import android.widget.AdapterView;
import android.widget.ArrayAdapter;
import android.widget.ListView;
import android.widget.Toast;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {
 ListView listView;
  String[] languages = {
       "Java",
       "Python",
       "C",
       "C++",
       "Kotlin",
       "PHP",
       "JavaScript",
       "Swift"
  };

  @Override
  protected void onCreate(Bundle savedInstanceState) {
       super.onCreate(savedInstanceState);
       setContentView(R.layout.activity_main);
       listView = findViewById(R.id.listView);
       ArrayAdapter<String> adapter = new ArrayAdapter<>(
         this,
         android.R.layout.simple_list_item_1,

             languages
        );
        listView.setAdapter(adapter);
        listView.setOnItemClickListener(new AdapterView.OnItemClickListener() {
             @Override
             public void onItemClick(AdapterView<?> parent, View view, int position, long id) {
        String item = languages[position];
        Toast.makeText(
        MainActivity.this,
        "Selected: " + item,
        Toast.LENGTH_SHORT

================== PAGE BREAK ==================

PAGE 62
        ).show();
              }
        });
    }
}

================== PAGE BREAK ==================

PAGE 63
Module 1 â€“ Practical 14
Develop an Android application using GridView with Custom Adapter

â† Back to Index

b )Develop an Android application using GridView with Custom Adapter
Project Name: GridViewDemo

I Filename: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout
 xmlns:android="http://schemas.android.com/apk/res/android"
  android:id="@+id/main"
  android:layout_width="match_parent"
  android:layout_height="match_parent"
  android:orientation="vertical"
  android:padding="10dp">

  <TextView
     android:layout_width="wrap_content"
     android:layout_height="wrap_content"
     android:paddingVertical="20dp"
     android:paddingBottom="10dp"
     android:text="Image Gallery"
     android:textSize="24sp"
     android:textStyle="bold" />

  <GridView
     android:id="@+id/gridView"
     android:layout_width="match_parent"
     android:layout_height="match_parent"
     android:numColumns="2"
     android:verticalSpacing="10dp"
     android:horizontalSpacing="10dp"

     android:stretchMode="columnWidth" />

</LinearLayout>

Create new layout file: resâ†’ layoutâ†’ New-> XML-> New Layout XML File->grid_item
II Filename: grid_item.xml

================== PAGE BREAK ==================

PAGE 64
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout
 xmlns:android="http://schemas.android.com/apk/res/android"
 android:layout_width="match_parent"
 android:layout_height="wrap_content"
 android:orientation="vertical"
 android:gravity="center"
 android:padding="10dp">

 <ImageView
   android:id="@+id/imageView"
   android:layout_width="120dp"
   android:layout_height="120dp"
   android:scaleType="centerCrop" />

 <TextView
   android:id="@+id/textView"
   android:layout_width="wrap_content"
   android:layout_height="wrap_content"
   android:textSize="18sp"
   android:paddingTop="5dp" />

</LinearLayout>

Create Custom Adapter Class. Right Click: java packageâ†’ New â†’ Java Classâ†’ Class
Name: CustomAdapter
III Filename: CustomAdapter.java

package com.example.gridviewdemo;
import android.content.Context;
import android.view.LayoutInflater;
import android.view.View;
import android.view.ViewGroup;
import android.widget.BaseAdapter;
import android.widget.ImageView;
import android.widget.TextView;

public class CustomAdapter extends BaseAdapter {
 Context context;
 String[] imageNames;
 int[] images;
 LayoutInflater inflater;
 public CustomAdapter(Context context, String[] imageNames, int[] images) {
     this.context = context;
     this.imageNames = imageNames;
     this.images = images;
     inflater = LayoutInflater.from(context);
 }

================== PAGE BREAK ==================

PAGE 65
    @Override
    public int getCount() {
        return imageNames.length;
    }

    @Override

     public Object getItem(int position) {
         return imageNames[position];
     }

     @Override
     public long getItemId(int position) {
         return position;
     }

     @Override
     public View getView(int position, View convertView, ViewGroup parent) {
         View view = inflater.inflate(R.layout.grid_item, parent, false);
         ImageView imageView = view.findViewById(R.id.imageView);
         TextView textView = view.findViewById(R.id.textView);
         imageView.setImageResource(images[position]);
         textView.setText(imageNames[position]);
         return view;
     }
}

Filename IV: MainActivity.java

package com.example.gridviewdemo;

import android.os.Bundle;
import android.widget.GridView;
import android.widget.Toast;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {
  private final String[] imageNames = {"Nature", "Flower", "Mountain", "Beach"};
  private final int[] images = {
     android.R.drawable.ic_menu_gallery,
     android.R.drawable.ic_menu_camera,
     android.R.drawable.ic_menu_compass,
     android.R.drawable.ic_menu_mapmode
  };

    @Override

================== PAGE BREAK ==================

PAGE 66
    protected void onCreate(Bundle savedInstanceState) {
      super.onCreate(savedInstanceState);
      setContentView(R.layout.activity_main);
      GridView gridView = findViewById(R.id.gridView);
      gridView.setAdapter(new CustomAdapter(this, imageNames, images));
      gridView.setOnItemClickListener((parent, view, position, id) ->
         Toast.makeText(this, "Selected: " + imageNames[position], Toast.LENGTH_SHORT).show());
    }
}

Module 1 â€“ Practical 15
Develop an Android application implementing RecyclerView as a modern alternative to
ListView.

â† Back to Index

c) Develop an Android application implementing RecyclerView as a modern alternative
to ListView.
Project Name : RecyclerViewDemo

Add RecyclerView Dependency. Open in android Project View, under Gradle Scripts:
build.gradle.kts (Module: app)
I Filename : Dependencies
dependencies {
    implementation libs.appcompat
    implementation libs.material
    implementation libs.activity
    implementation libs.constraintlayout
    testImplementation libs.junit
    androidTestImplementation libs.ext.junit
    androidTestImplementation libs.espresso.core
    implementation("androidx.recyclerview:recyclerview:1.3.2")
}

II Filename: activity_main.xml
<?xml version="1.0" encoding="utf-8"?>

<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:padding="10dp">

     <TextView
       android:layout_width="wrap_content"

================== PAGE BREAK ==================

PAGE 67
   android:layout_height="wrap_content"
   android:layout_marginVertical="50dp"
   android:paddingBottom="10dp"
   android:text="RecyclerView Demo"
   android:textSize="24sp"
   android:textStyle="bold" />

  <androidx.recyclerview.widget.RecyclerView
    android:id="@+id/recyclerView"
    android:layout_width="match_parent"
    android:layout_height="match_parent" />
</LinearLayout>

Create Item Layout. Create:resâ†’ layout â†’ New-> XML-> New Layout XML File->
item_layout

III Filename: item_layout.xml

<?xml version="1.0" encoding="utf-8"?>
<TextView
     xmlns:android="http://schemas.android.com/apk/res/android"
     android:id="@+id/txtItem"
     android:layout_width="match_parent"
     android:layout_height="wrap_content"
     android:textSize="20sp"
     android:padding="15dp"/>

Create Adapter Class java packageâ†’ New â†’ Java Class Right Click: â†’ Class Name:
MyAdapter

IV Filename: MyAdapter.java

package com.example.recyclerviewdemo;
import android.view.LayoutInflater;
import android.view.View;
import android.view.ViewGroup;
import android.widget.TextView;
import android.widget.Toast;
import androidx.annotation.NonNull;
import androidx.recyclerview.widget.RecyclerView;

================== PAGE BREAK ==================

PAGE 68
public class MyAdapter extends RecyclerView.Adapter<MyAdapter.ViewHolder> {
  String[] data;
  public MyAdapter(String[] data) {
      this.data = data;
  }

    public static class ViewHolder extends RecyclerView.ViewHolder {
        TextView txtItem;
        public ViewHolder(@NonNull View itemView) {
            super(itemView);
            txtItem = itemView.findViewById(R.id.txtItem);
        }
    }

    @NonNull
    @Override
    public ViewHolder onCreateViewHolder(@NonNull ViewGroup parent, int viewType) {

          View view = LayoutInflater.from(parent.getContext()).inflate(
               R.layout.item_layout,
               parent,
               false
          );
          return new ViewHolder(view);
      }

      @Override
      public void onBindViewHolder(@NonNull ViewHolder holder, int position) {
          holder.txtItem.setText(data[position]);
          holder.itemView.setOnClickListener(v -> {
               Toast.makeText(
        v.getContext(),
        "Selected: " + data[position],
        Toast.LENGTH_SHORT
               ).show();
          });
      }
      @Override
      public int getItemCount() {
          return data.length;
      }
}

V Filename: Main_Activity.java

package com.example.recyclerviewdemo;
import android.os.Bundle;
import androidx.appcompat.app.AppCompatActivity;
import androidx.recyclerview.widget.LinearLayoutManager;

================== PAGE BREAK ==================

PAGE 69
import androidx.recyclerview.widget.RecyclerView;
public class MainActivity extends AppCompatActivity {

    RecyclerView recyclerView;
    String[] languages = {
         "Java",
         "Python",
         "C",
         "C++",
         "Kotlin",
         "PHP",
         "JavaScript",
         "Swift",
         "Go",
         "Ruby"
    };
    @Override
    protected void onCreate(Bundle savedInstanceState) {
         super.onCreate(savedInstanceState);
         setContentView(R.layout.activity_main);

        recyclerView = findViewById(R.id.recyclerView);
        recyclerView.setLayoutManager(new LinearLayoutManager(this));
        MyAdapter adapter = new MyAdapter(languages);
        recyclerView.setAdapter(adapter);
    }
}

================== PAGE BREAK ==================

PAGE 70
Module 2 â€“ Practical 1
Develop an Android application implementing AppBar (Toolbar) and Options Menu.

â† Back to Index

        Menus, Dialogs and UI Interaction

1. Develop an Android application implementing AppBar (Toolbar) and Options Menu.

Project Name: ToolbarMenuDemo

FileName: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

 xmlns:android="http://schemas.android.com/apk/res/android"
xmlns:app="http://schemas.android.com/apk/res-auto"

    android:id="@+id/main"

    android:layout_width="match_parent"

    android:layout_height="match_parent" android:orientation="vertical">

    <!-- Toolbar -->

    <androidx.appcompat.widget.Toolbar

       android:id="@+id/toolbar"

       android:layout_width="match_parent"

       android:layout_height="?attr/actionBarSize"

       android:background="?attr/colorPrimary"

================== PAGE BREAK ==================

PAGE 71
      app:title="Toolbar Demo"

      app:titleTextColor="@android:color/white"/>

   <!--Main Content -->

   <TextView

      android:layout_width="wrap_content"

      android:layout_height="wrap_content"

      android:text="AppBar and Options Menu Example"

      android:textSize="22sp"

      android:padding="20dp"/>

</LinearLayout>

Create a Menu Resource File.
Right Click: Res â†’ Newâ†’ Android Resource Directory

Directory Name: menu
Resource Type: menu

Create Menu XML File.
Right Click: menu Newâ†’ Menu Resource File Give name as menu_main.xml

File Name : menu_main.xml

<?xml version="1.0" encoding="utf-8"?>

<menu xmlns:android="http://schemas.android.com/apk/res/android"

   xmlns:app="http://schemas.android.com/apk/res-auto">

================== PAGE BREAK ==================

PAGE 72
   <item

      android:id="@+id/menu_home"

      android:title="Home"

      app:showAsAction="never"/>

   <item

      android:id="@+id/menu_settings"

      android:title="Settings"

      app:showAsAction="never"/>

   <item

      android:id="@+id/menu_about"

      android:title="About"

      app:showAsAction="never"/>

   <item

      android:id="@+id/menu_logout"

      android:title="Logout"

      app:showAsAction="never"/>

</menu>

================== PAGE BREAK ==================

PAGE 73
File Name: MainActivity.java.

package com.example.toolbarmenudemo;

import android.os.Bundle;

import android.view.Menu;

import android.view.MenuItem;

import android.widget.Toast;

import androidx.annotation.NonNull;

import androidx.appcompat.app.AppCompatActivity;

import androidx.appcompat.widget.Toolbar;

public class MainActivity extends AppCompatActivity {

================== PAGE BREAK ==================

PAGE 74
Toolbar toolbar;

 @Override

 protected void onCreate(Bundle savedInstanceState) {

      super.onCreate(savedInstanceState);

      setContentView(R.layout.activity_main);

      toolbar = findViewById(R.id.toolbar);

      // Set Toolbar as AppBar

      setSupportActionBar(toolbar);

 }

// Create Options Menu

 @Override

 public boolean onCreateOptionsMenu(Menu menu) {

      getMenuInflater().inflate(R.menu.menu_main, menu);

      return true;

  }

  // Handle Menu Item Click

  @Override

  public boolean onOptionsItemSelected(@NonNull MenuItem item) {

      int id = item.getItemId();

      if (id == R.id.menu_home) {

================== PAGE BREAK ==================

PAGE 75
            Toast.makeText(this, "Home Selected", Toast.LENGTH_SHORT).show();

        } else if (id == R.id.menu_settings) {

            Toast.makeText(this, "Settings Selected",
Toast.LENGTH_SHORT).show();

        } else if (id == R.id.menu_about) {

            Toast.makeText(this, "About Selected", Toast.LENGTH_SHORT).show();

        } else if (id == R.id.menu_logout) {

            Toast.makeText(this, "Logout Selected", Toast.LENGTH_SHORT).show();

        }

        return true;

    }

}

================== PAGE BREAK ==================

PAGE 76
Module 2 â€“ Practical 2
Develop an Android application demonstrating AlertDialog and custom DialogFragment.

â† Back to Index

2. Develop an Android application demonstrating AlertDialog and custom
DialogFragment.

ProjectName: DialogDemo

File Name: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

 xmlns:android="http://schemas.android.com/apk/res/android"

   android:id="@+id/main"

   android:layout_width="match_parent" android:layout_height="match_parent"

   android:orientation="vertical"

   android:gravity="center" android:padding="20dp">

   <Button

       android:id="@+id/btnAlert"

       android:layout_width="wrap_content"

       android:layout_height="wrap_content"

       android:text="Show AlertDialog"/>

================== PAGE BREAK ==================

PAGE 77
  <Button

      android:id="@+id/btnCustom" android:layout_width="wrap_content"

      android:layout_height="wrap_content" android:text="Show Custom Dialog"

      android:layout_marginTop="20dp"/>

</LinearLayout>

Create Custom Dialog Layout.
Create:
resâ†’ layout â†’ New-> XML-> New Layout XML File â†’ dialog_custom

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

 xmlns:android="http://schemas.android.com/apk/res/android"

 android:layout_width="match_parent"

 android:layout_height="wrap_content"

 android:orientation="vertical"

 android:padding="20dp">

 <TextView

      android:layout_width="wrap_content"

      android:layout_height="wrap_content"

      android:text="Custom DialogFragment"

      android:textSize="22sp"

================== PAGE BREAK ==================

PAGE 78
     android:textStyle="bold"/>

 <EditText

     android:id="@+id/etName"

     android:layout_width="match_parent"

     android:layout_height="wrap_content"

     android:hint="Enter Name"

     android:layout_marginTop="15dp"/>

</LinearLayout>

Create Dialog Fragment Class.
Right Click: java package â†’ New â†’ Java Class

Class Name: CustomDialogFragment.java

package com.example.dialogdemo;

import android.app.AlertDialog;

import android.app.Dialog;

import android.os.Bundle;

import android.view.LayoutInflater;

import android.view.View;

import android.widget.EditText;

================== PAGE BREAK ==================

PAGE 79
import android.widget.Toast;

import androidx.annotation.NonNull;

import androidx.fragment.app.DialogFragment;

public class CustomDialogFragment extends DialogFragment {

 EditText etName;

 @NonNull

  @Override

  public Dialog onCreateDialog(Bundle savedInstanceState) {

      AlertDialog.Builder builder = new AlertDialog.Builder(getActivity());

      LayoutInflater inflater = requireActivity().getLayoutInflater();

      View view = inflater.inflate(R.layout.dialog_custom, null);

       etName = view.findViewById(R.id.etName);

       builder.setView(view)

               .setTitle("Custom Dialog")

================== PAGE BREAK ==================

PAGE 80
        .setPositiveButton("Submit", (dialog, which) -> {

        String name = etName.getText().toString();

        Toast.makeText(getActivity(),

        "Entered: " + name,

        Toast.LENGTH_SHORT).show();

        })

                .setNegativeButton("Cancel", (dialog, which) ->
dialog.dismiss());

        return builder.create();

    }

}

FileName: MainActivity.java

package com.example.dialogdemo;

import android.os.Bundle;

import android.widget.Button;

import android.widget.Toast;

================== PAGE BREAK ==================

PAGE 81
import androidx.appcompat.app.AlertDialog;

import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

 Button btnAlert, btnCustom;

 @Override

 protected void onCreate(Bundle savedInstanceState) {

     super.onCreate(savedInstanceState);

     setContentView(R.layout.activity_main);

     btnAlert = findViewById(R.id.btnAlert);

     btnCustom = findViewById(R.id.btnCustom);

     // AlertDialog Example

     btnAlert.setOnClickListener(v -> {

          AlertDialog.Builder builder = new AlertDialog.Builder(this);

          builder.setTitle("Delete File")

================== PAGE BREAK ==================

PAGE 82
        .setMessage("Are you sure you want to delete?")

        .setPositiveButton("YES", (dialog, which) -> {

        Toast.makeText(this,

        "File Deleted",

        Toast.LENGTH_SHORT).show();

        })

        .setNegativeButton("NO", (dialog, which) ->
dialog.dismiss());

               builder.show();

        });

        // Custom Dialog Example

        btnCustom.setOnClickListener(v -> {

               CustomDialogFragment dialog = new CustomDialogFragment();

               dialog.show(getSupportFragmentManager(), "CustomDialog");

        });

    }

}

================== PAGE BREAK ==================

PAGE 83
Module 2 â€“ Practical 3
Develop an Android application implementing contextual menus and popup menus.

â† Back to Index

3. Develop an Android application implementing contextual menus and popup menus.

ProjectName: MenuDemo

File Name: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

 xmlns:android="http://schemas.android.com/apk/res/android"

   android:layout_width="match_parent"

   android:layout_height="match_parent"

   android:orientation="vertical"

   android:gravity="center"

   android:padding="20dp">

   <TextView

       android:id="@+id/txtContext"

       android:layout_width="wrap_content"

       android:layout_height="wrap_content"

       android:text="Long Press Me"

       android:textSize="24sp"

       android:padding="20dp"/>

================== PAGE BREAK ==================

PAGE 84
  <Button

      android:id="@+id/btnPopup"

      android:layout_width="wrap_content"

      android:layout_height="wrap_content"

      android:text="Show Popup Menu"

      android:layout_marginTop="30dp"/>

</LinearLayout>

Create a Menu Resource File.
Right Click: resâ†’ New â†’ Android Resource Directory
Directory Name: menu
Resource Type: menu
Click OK
Right Click: menu â†’ New â†’ Menu Resource File

File Name : menu_options

File Name : menu_options.xml

<?xml version="1.0" encoding="utf-8"?>

<menu xmlns:android="http://schemas.android.com/apk/res/android">

  <item

      android:id="@+id/menu_edit" android:title="Edit"/>

================== PAGE BREAK ==================

PAGE 85
   <item

       android:id="@+id/menu_delete"

       android:title="Delete"/>

   <item

       android:id="@+id/menu_share"

       android:title="Share"/>

</menu>

File Name: MainActivity.java

package com.example.menudemo;

import android.os.Bundle;

import android.view.ContextMenu;

import android.view.MenuItem;

import android.view.View;

import android.widget.Button;

import android.widget.PopupMenu;

import android.widget.TextView;

import android.widget.Toast;

================== PAGE BREAK ==================

PAGE 86
import androidx.annotation.NonNull;

import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

 TextView txtContext;

 Button btnPopup;

 @Override

 protected void onCreate(Bundle savedInstanceState) {

     super.onCreate(savedInstanceState);

     setContentView(R.layout.activity_main);

     txtContext = findViewById(R.id.txtContext);

     btnPopup = findViewById(R.id.btnPopup);

     // Register Context Menu

================== PAGE BREAK ==================

PAGE 87
registerForContextMenu(txtContext);

// Popup Menu

btnPopup.setOnClickListener(v -> {

    PopupMenu popupMenu = new PopupMenu(MainActivity.this, btnPopup);

    popupMenu.getMenuInflater().inflate(

            R.menu.menu_options,

            popupMenu.getMenu());

    popupMenu.setOnMenuItemClickListener(item -> {

          Toast.makeText(MainActivity.this,

        item.getTitle(),

        Toast.LENGTH_SHORT).show();

          return true;

    });

================== PAGE BREAK ==================

PAGE 88
            popupMenu.show();

    });

}

// Context Menu Creation

@Override

public void onCreateContextMenu(ContextMenu menu,

        View v,

        ContextMenu.ContextMenuInfo menuInfo) {

    super.onCreateContextMenu(menu, v, menuInfo);

    menu.setHeaderTitle("Select Option");

    getMenuInflater().inflate(R.menu.menu_options, menu);

}

================== PAGE BREAK ==================

PAGE 89
// Context Menu Click Handling

@Override

public boolean onContextItemSelected(@NonNull MenuItem item) {

        Toast.makeText(this,

               item.getTitle(),

               Toast.LENGTH_SHORT).show();

        return true;

    }

}

================== PAGE BREAK ==================

PAGE 90
Module 2 â€“ Practical 4
Develop an Android application implementing Explicit and Implicit Intents.

â† Back to Index

        Intents, Events and Listeners

4. Develop an Android application implementing Explicit and Implicit Intents.

ProjectName: IntentDemo

File Name: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

    xmlns:android="http://schemas.android.com/apk/res/android"

    android:layout_width="match_parent" android:layout_height="match_parent"

    android:orientation="vertical"

    android:gravity="center"

    android:id="@+id/main"

    android:padding="20dp">

    <Button

       android:id="@+id/btnExplicit"

       android:layout_width="wrap_content"

       android:layout_height="wrap_content"

================== PAGE BREAK ==================

PAGE 91
       android:text="Explicit Intent"/>

    <Button

       android:id="@+id/btnImplicit"

       android:layout_width="wrap_content"

       android:layout_height="wrap_content" android:text="Implicit Intent"

       android:layout_marginTop="20dp"/>

</LinearLayout>

Create Second Activity.

Right Click: java package â†’ com.example.projectname -> Newâ†’ Activity â†’ Empty Views
Activity

Activity Name: SecondActivity
Click: Finish

Design Second Activity Layout.
Open: resâ†’ layout â†’ activity_second.xml

File Name: activity_second.xml

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

    xmlns:android="http://schemas.android.com/apk/res/android"

    android:layout_width="match_parent"

    android:layout_height="match_parent"

    android:id="@+id/main"

================== PAGE BREAK ==================

PAGE 92
    android:gravity="center">

    <TextView

       android:layout_width="wrap_content"

       android:layout_height="wrap_content"

       android:text="Welcome to Second Activity"

       android:textSize="24sp"/>

</LinearLayout>

File Name: MainActivity.java.

package com.example.intentdemo;

import android.content.Intent;

import android.net.Uri;

import android.os.Bundle;

import android.widget.Button;

import androidx.appcompat.app.AppCompatActivity;

================== PAGE BREAK ==================

PAGE 93
public class MainActivity extends AppCompatActivity {

 Button btnExplicit, btnImplicit;

  @Override

  protected void onCreate(Bundle savedInstanceState) {

        super.onCreate(savedInstanceState);

        setContentView(R.layout.activity_main);

        btnExplicit = findViewById(R.id.btnExplicit);

        btnImplicit = findViewById(R.id.btnImplicit);

        // Explicit Intent

        btnExplicit.setOnClickListener(v -> {

               Intent intent = new Intent(MainActivity.this, SecondActivity.class);

               startActivity(intent);

================== PAGE BREAK ==================

PAGE 94
        });

        // Implicit Intent

        btnImplicit.setOnClickListener(v -> {

              Intent intent = new Intent(

        Intent.ACTION_VIEW,

        Uri.parse("https://www.google.com")

              );

              startActivity(intent);

        });

    }

}

================== PAGE BREAK ==================

PAGE 95
Module 2 â€“ Practical 5
Develop an Android application demonstrating Event Handling using Listeners (OnClick,
OnLongClick, etc.).

â† Back to Index

5. Develop an Android application demonstrating Event Handling using Listeners
(OnClick, OnLongClick, etc.).

Project Name: EventHandlingDemo

File Name: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

 xmlns:android="http://schemas.android.com/apk/res/android"

   android:layout_width="match_parent"

   android:layout_height="match_parent"

   android:orientation="vertical"

   android:gravity="center"

   android:padding="20dp">

   <Button

       android:id="@+id/btnClick"

       android:layout_width="wrap_content"

       android:layout_height="wrap_content"

       android:text="Click Me"/>

   <Button

================== PAGE BREAK ==================

PAGE 96
       android:id="@+id/btnLongClick"

       android:layout_width="wrap_content"

       android:layout_height="wrap_content"

       android:text="Long Press Me"

       android:layout_marginTop="20dp"/>

</LinearLayout>

File Name: MainActivity.java

package com.example.eventhandlingdemo;

import android.os.Bundle;

import android.widget.Button;

import android.widget.Toast;

import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

================== PAGE BREAK ==================

PAGE 97
Button btnClick, btnLongClick;

 @Override

 protected void onCreate(Bundle savedInstanceState) {

     super.onCreate(savedInstanceState);

     setContentView(R.layout.activity_main);

     btnClick = findViewById(R.id.btnClick);

     btnLongClick = findViewById(R.id.btnLongClick);

     // OnClickListener

     btnClick.setOnClickListener(v -> {

          Toast.makeText(

        MainActivity.this,

        "Button Clicked",

        Toast.LENGTH_SHORT

             ).show();

================== PAGE BREAK ==================

PAGE 98
        });

        // OnLongClickListener

        btnLongClick.setOnLongClickListener(v -> {

              Toast.makeText(

        MainActivity.this,

        "Button Long Pressed",

        Toast.LENGTH_SHORT

              ).show();

              return true;

        });

    }

}

================== PAGE BREAK ==================

PAGE 99
Module 2 â€“ Practical 6
Develop an Android application using Adapters to populate Spinner or ListView
dynamically.

â† Back to Index

6. Develop an Android application using Adapters to populate Spinner or ListView
dynamically.

Android Spinner is a view similar to the dropdown list which is used to select one option
from the list of options. It provides an easy way to select one item from the list of items
and it shows a dropdown list of all values when we click on it. The default value of the
android spinner will be the currently selected value and by using Adapter we can easily
bind the items to the spinner objects. Generally, we populate our Spinner control with a
list of items by using an ArrayAdapter in our Kotlin/Java file.

Project Name: AdapterDemo

File Name: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

 xmlns:android="http://schemas.android.com/apk/res/android"

   android:layout_width="match_parent"

   android:layout_height="match_parent"

   android:orientation="vertical"

   android:padding="20dp">

   <Spinner

        android:id="@+id/spinner"

        android:layout_width="match_parent"

        android:layout_height="wrap_content"/>

================== PAGE BREAK ==================

PAGE 100
   <ListView

        android:id="@+id/listView"

        android:layout_width="match_parent"

        android:layout_height="wrap_content"

        android:layout_marginTop="20dp"/>

</LinearLayout>

File Name: MainActivity.java

package com.example.adapterdemo;

import android.os.Bundle;

import android.view.View;

import android.widget.AdapterView;

import android.widget.ArrayAdapter;

import android.widget.ListView;

import android.widget.Spinner;

import android.widget.Toast;

import androidx.appcompat.app.AppCompatActivity;

================== PAGE BREAK ==================

PAGE 101
public class MainActivity extends AppCompatActivity {

 Spinner spinner;

 ListView listView;

 String[] cities = {

             "Mumbai",

             "Pune",

             "Delhi",

             "Chennai",

             "Hyderabad"

  };

 @Override

 protected void onCreate(Bundle savedInstanceState) {

       super.onCreate(savedInstanceState);

       setContentView(R.layout.activity_main);

================== PAGE BREAK ==================

PAGE 102
spinner = findViewById(R.id.spinner);

listView = findViewById(R.id.listView);

// Spinner Adapter

ArrayAdapter<String> spinnerAdapter = new ArrayAdapter<>(

        this,

        android.R.layout.simple_spinner_dropdown_item,

        cities

);

spinner.setAdapter(spinnerAdapter);

// ListView Adapter

ArrayAdapter<String> listAdapter = new ArrayAdapter<>(

        this,

        android.R.layout.simple_list_item_1,

        cities

);

listView.setAdapter(listAdapter);

================== PAGE BREAK ==================

PAGE 103
     // Spinner Item Selection

      spinner.setOnItemSelectedListener(new
AdapterView.OnItemSelectedListener() {

             @Override

             public void onItemSelected(AdapterView<?> parent, View view,

        int position, long id) {

        Toast.makeText(

        MainActivity.this,

        "Selected: " + cities[position],

        Toast.LENGTH_SHORT

        ).show();

             }

             @Override

             public void onNothingSelected(AdapterView<?> parent) {

             }

       });

       // ListView Item Click

================== PAGE BREAK ==================

PAGE 104
        listView.setOnItemClickListener((parent, view, position, id) -> {

              Toast.makeText(

        MainActivity.this,

        "Clicked: " + cities[position],

        Toast.LENGTH_SHORT

              ).show();

        });

    }

}

================== PAGE BREAK ==================

PAGE 105
Module 2 â€“ Practical 7
Develop an Android application implementing Started and Bound Services.

â† Back to Index

        Services, Notifications and Broadcast Receivers

7. Develop an Android application implementing Started and Bound Services.

A bound service is the server in a client-server interface. It lets components such as
activities bind to the service, send requests, receive responses, and perform
interprocess communication (IPC). A bound service typically lives only while it serves
another application component and does not run in the background indefinitely.

Project Name: ServiceDemo

File Name: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

 xmlns:android="http://schemas.android.com/apk/res/android"

   android:layout_width="match_parent"

   android:layout_height="match_parent"

   android:orientation="vertical"

   android:gravity="center"

   android:padding="20dp">

   <Button

       android:id="@+id/btnStart"

       android:layout_width="wrap_content"

================== PAGE BREAK ==================

PAGE 106
       android:layout_height="wrap_content"

       android:text="Start Service"/>

   <Button

       android:id="@+id/btnStop"

       android:layout_width="wrap_content"

       android:layout_height="wrap_content"

       android:text="Stop Service"

       android:layout_marginTop="15dp"/>

   <Button

       android:id="@+id/btnBound"

       android:layout_width="wrap_content"

       android:layout_height="wrap_content"

       android:text="Bind Service"

       android:layout_marginTop="15dp"/>

</LinearLayout>

Create a Started Service Class.

Right Click: java packageâ†’ New â†’ Java Class

Class Name: MyStartedService

================== PAGE BREAK ==================

PAGE 107
File Name: MyStartedService.java

package com.example.servicedemo;

import android.app.Service;

import android.content.Intent;

import android.os.IBinder;

import android.widget.Toast;

public class MyStartedService extends Service {

  @Override

  public int onStartCommand(Intent intent, int flags, int startId) {

       Toast.makeText(

               this,

               "Started Service Running",

               Toast.LENGTH_SHORT

       ).show();

================== PAGE BREAK ==================

PAGE 108
    return START_STICKY;

}

@Override

public void onDestroy() {

    super.onDestroy();

    Toast.makeText(

            this,

            "Started Service Stopped",

            Toast.LENGTH_SHORT

    ).show();

}

@Override

================== PAGE BREAK ==================

PAGE 109
    public IBinder onBind(Intent intent) {

        return null;

    }

}

Create a Bound Service Class (Similar like above).

Create Java Class: MyBoundService

File Name:MyBoundService

package com.example.servicedemo;

import android.app.Service;

import android.content.Intent;

import android.os.Binder;

import android.os.IBinder;

public class MyBoundService extends Service {

    private final IBinder binder = new LocalBinder();

================== PAGE BREAK ==================

PAGE 110
    public class LocalBinder extends Binder {

        public MyBoundService getService() {

            return MyBoundService.this;

        }

    }

    @Override

    public IBinder onBind(Intent intent) {

        return binder;

    }

    public String getMessage() {

        return "Bound Service Connected";

    }

}

================== PAGE BREAK ==================

PAGE 111
File Name: MainActivity.java

package com.example.servicedemo;

import android.content.ComponentName;

import android.content.Intent;

import android.content.ServiceConnection;

import android.os.Bundle;

import android.os.IBinder;

import android.widget.Button;

import android.widget.Toast;

import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

================== PAGE BREAK ==================

PAGE 112
   Button btnStart, btnStop, btnBound;

   MyBoundService myBoundService;

   boolean isBound = false;

   @Override

protected void onCreate(Bundle savedInstanceState) {

 super.onCreate(savedInstanceState);

  setContentView(R.layout.activity_main);

 btnStart = findViewById(R.id.btnStart);

 btnStop = findViewById(R.id.btnStop);

 btnBound = findViewById(R.id.btnBound);

================== PAGE BREAK ==================

PAGE 113
// Start Service

btnStart.setOnClickListener(v -> {

        Intent intent = new Intent(

        this,

        MyStartedService.class

        );

        startService(intent);

 });

// Stop Service

btnStop.setOnClickListener(v -> {

================== PAGE BREAK ==================

PAGE 114
      Intent intent = new Intent(

             this,

               MyStartedService.class

       );

       stopService(intent);

});

// Bind Service

btnBound.setOnClickListener(v -> {

       Intent intent = new Intent(

               this,

               MyBoundService.class

       );

       bindService(

               intent,

================== PAGE BREAK ==================

PAGE 115
        serviceConnection,

        BIND_AUTO_CREATE

          );

    });

}

// Service Connection

ServiceConnection serviceConnection = new ServiceConnection() {

    @Override

    public void onServiceConnected(

        ComponentName name,

        IBinder service) {

               MyBoundService.LocalBinder binder =

        (MyBoundService.LocalBinder) service;

               myBoundService = binder.getService();

               isBound = true;

               Toast.makeText(

        MainActivity.this,

        myBoundService.getMessage(),

================== PAGE BREAK ==================

PAGE 116
        Toast.LENGTH_SHORT

             ).show();

         }

         @Override

         public void onServiceDisconnected(ComponentName name) {

             isBound = false;

         }

    };

    @Override

    protected void onDestroy() {

         super.onDestroy();

         if (isBound) {

             unbindService(serviceConnection);

             isBound = false;

         }

    }

}

Add Services in AndroidManifest.xml (in Android Project Panel).

================== PAGE BREAK ==================

PAGE 117
Open:

appâ†’ Manifests â†’ AndroidManifest.xml

Inside: <application>

Add:->

<service android:name=".MyStartedService"/>

<service android:name=".MyBoundService"/>

================== PAGE BREAK ==================

PAGE 118
Module 2 â€“ Practical 8
Develop an Android application implementing Notifications using Notification Manager.

â† Back to Index

8. Develop an Android application implementing Notifications using Notification Manager.

Project Name: NotificationDemo

File Name: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

 xmlns:android="http://schemas.android.com/apk/res/android"

   android:layout_width="match_parent"

   android:layout_height="match_parent"

   android:gravity="center">

   <Button

       android:id="@+id/btnNotify"

       android:layout_width="wrap_content"

       android:layout_height="wrap_content"

       android:text="Show Notification"/>

</LinearLayout>

Add Permission in Manifest,

================== PAGE BREAK ==================

PAGE 119
Open: AndroidManifest.xml

Add above <application>:

<uses-permission android:name="android.permission.POST_NOTIFICATIONS"/>

File Name: MainActivity.java

package com.example.notificationdemo;

import android.Manifest;

import android.app.NotificationChannel;

import android.app.NotificationManager;

import android.content.pm.PackageManager;

import android.os.Build;

import android.os.Bundle;

import android.widget.Button;

import androidx.appcompat.app.AppCompatActivity;

import androidx.core.app.NotificationCompat;

public class MainActivity extends AppCompatActivity {

================== PAGE BREAK ==================

PAGE 120
private static final String CHANNEL_ID = "MyChannel";

private static final int NOTIFICATION_PERMISSION_CODE = 100;

private Button btnNotify;

@Override

protected void onCreate(Bundle savedInstanceState) {

    super.onCreate(savedInstanceState);

    setContentView(R.layout.activity_main);

// Find the button from activity_main.xml

btnNotify = findViewById(R.id.btnNotify);

// Create notification channel

createNotificationChannel();

================== PAGE BREAK ==================

PAGE 121
    // Request notification permission for Android 13+

    requestNotificationPermission();

    // Button click

    btnNotify.setOnClickListener(v -> {

          showNotification();

    });

}

// Request notification permission

private void requestNotificationPermission() {

    if (Build.VERSION.SDK_INT >= Build.VERSION_CODES.TIRAMISU) {

          if (checkSelfPermission(Manifest.permission.POST_NOTIFICATIONS)

================== PAGE BREAK ==================

PAGE 122
        != PackageManager.PERMISSION_GRANTED) {

              requestPermissions(

        new String[]{Manifest.permission.POST_NOTIFICATIONS},

        NOTIFICATION_PERMISSION_CODE

              );

        }

    }

}

// Create notification channel

private void createNotificationChannel() {

    if (Build.VERSION.SDK_INT >= Build.VERSION_CODES.O) {

        NotificationChannel channel = new NotificationChannel(

================== PAGE BREAK ==================

PAGE 123
        CHANNEL_ID,

        "My Channel",

        NotificationManager.IMPORTANCE_DEFAULT

        );

        channel.setDescription("Notification Channel for Demo");

        NotificationManager manager =

        getSystemService(NotificationManager.class);

        if (manager != null) {

              manager.createNotificationChannel(channel);

        }

    }

}

// Show notification

private void showNotification() {

================== PAGE BREAK ==================

PAGE 124
// Check permission for Android 13+

if (Build.VERSION.SDK_INT >= Build.VERSION_CODES.TIRAMISU) {

     if (checkSelfPermission(Manifest.permission.POST_NOTIFICATIONS)

              != PackageManager.PERMISSION_GRANTED) {

         requestNotificationPermission();

         return;

     }

 }

NotificationCompat.Builder builder =

         new NotificationCompat.Builder(this, CHANNEL_ID)

        .setSmallIcon(android.R.drawable.ic_dialog_info)

        .setContentTitle("Notification Example")

================== PAGE BREAK ==================

PAGE 125
        .setContentText("Hello from Android Notification")

        .setPriority(NotificationCompat.PRIORITY_DEFAULT)

        .setAutoCancel(true);

    NotificationManager manager =

              (NotificationManager) getSystemService(NOTIFICATION_SERVICE);

          if (manager != null) {

              manager.notify(1, builder.build());

          }

      }

}

================== PAGE BREAK ==================

PAGE 126
Module 2 â€“ Practical 9
Develop an Android application implementing Static and Dynamic Broadcast Receivers.

â† Back to Index

9. Develop an Android application implementing Static and Dynamic Broadcast
Receivers.

Project Name: BroadcastDemo

File Name: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"

  android:layout_width="match_parent"
  android:layout_height="match_parent"

  android:gravity="center"
  android:orientation="vertical"

  android:padding="24dp">
  <TextView

    android:layout_width="wrap_content"
    android:layout_height="wrap_content"

    android:text="Broadcast Receiver Example"
    android:textSize="22sp" />

  <Button
    android:id="@+id/btnBroadcast"

    android:layout_width="wrap_content"
    android:layout_height="wrap_content"

    android:layout_marginTop="20dp"
    android:text="Send Broadcast" />

</LinearLayout>

Create a Broadcast Receiver Class.

Right Click:-> java package â†’ New â†’ Java Class Class Name: MyReceiver

================== PAGE BREAK ==================

PAGE 127
package com.example.broadcastdemo;

import android.content.BroadcastReceiver;

import android.content.Context;

import android.content.Intent;

import android.widget.Toast;

public class MyReceiver extends BroadcastReceiver {

    @Override

    public void onReceive(Context context, Intent intent) {

        Toast.makeText(

                context,

                "Broadcast Received",

                Toast.LENGTH_SHORT

        ).show();

    }

}

Static Broadcast Receiver.

================== PAGE BREAK ==================

PAGE 128
Open:AndroidManifest.xml

Inside: <application>

Add:

<receiver
  android:name=".MyReceiver"

  android:exported="false">
  <intent-filter>

     <action android:name="com.example.broadcastdemo.CUSTOM_BROADCAST" />
  </intent-filter>

</receiver>

Dynamic Broadcast Receiver.

File Name: MainActivity.java

package com.example.broadcastdemo;

import android.content.Intent;
import android.content.IntentFilter;

import android.os.Bundle;
import android.widget.Button;

import androidx.appcompat.app.AppCompatActivity;
import androidx.core.content.ContextCompat;

public class MainActivity extends AppCompatActivity {

  private final MyReceiver myReceiver = new MyReceiver();

  private boolean receiverRegistered = false;

  @Override
  protected void onCreate(Bundle savedInstanceState) {

       super.onCreate(savedInstanceState);

       setContentView(R.layout.activity_main);

       IntentFilter filter = new IntentFilter("com.example.broadcastdemo.CUSTOM_BROADCAST");

================== PAGE BREAK ==================

PAGE 129
    ContextCompat.registerReceiver(this, myReceiver, filter,
ContextCompat.RECEIVER_NOT_EXPORTED);
    receiverRegistered = true;

        Button btnBroadcast = findViewById(R.id.btnBroadcast);

        btnBroadcast.setOnClickListener(v -> {

              Intent intent = new Intent(this, MyReceiver.class);

              intent.setAction("com.example.broadcastdemo.CUSTOM_BROADCAST");
              sendBroadcast(intent);

        });
    }

    @Override

    protected void onDestroy() {
      if (receiverRegistered) {

              unregisterReceiver(myReceiver);

              receiverRegistered = false;

        }

        super.onDestroy();
    }

}

Tap Send Broadcast. The registered dynamic receiver and the manifest receiver demonstrate broadcast
delivery; the manifest receiver uses an explicit in-app broadcast to avoid modern Android restrictions on
system broadcasts.

================== PAGE BREAK ==================

PAGE 130
Module 2 â€“ Practical 10
Develop an Android application implementing SQLite database CRUD operations.

â† Back to Index

        Database and Networking

 10. Develop an Android application implementing SQLite database CRUD operations.

ProjectName: SQLLiteCRUDDemo

File Name: activity_main.xml

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

 xmlns:android="http://schemas.android.com/apk/res/android"

   android:layout_width="match_parent"

   android:layout_height="match_parent"

   android:orientation="vertical"

   android:padding="20dp">

   <EditText

       android:id="@+id/etName"

       android:layout_width="match_parent"

       android:layout_height="wrap_content"

       android:hint="Enter Name"/>

   <EditText

       android:id="@+id/etNewName"

================== PAGE BREAK ==================

PAGE 131
     android:layout_width="match_parent"

     android:layout_height="wrap_content"

     android:hint="Enter New Name"/>

 <Button

     android:id="@+id/btnInsert"

     android:layout_width="match_parent"

     android:layout_height="wrap_content"

    android:text="Insert"/>

<Button

    android:id="@+id/btnView"

    android:layout_width="match_parent"

    android:layout_height="wrap_content"

    android:text="View Data"/>

<Button

    android:id="@+id/btnUpdate"

    android:layout_width="match_parent"

    android:layout_height="wrap_content"

    android:text="Update"/>

<Button

    android:id="@+id/btnDelete"

================== PAGE BREAK ==================

PAGE 132
      android:layout_width="match_parent"

      android:layout_height="wrap_content"

      android:text="Delete"/>

  <TextView

      android:id="@+id/txtResult" android:layout_width="match_parent"

      android:layout_height="wrap_content"

      android:textSize="18sp"

       android:paddingTop="20dp"/>

</LinearLayout>

Create a Database Helper Class.

Right Click:

java package â†’ New â†’ Java Class

Class Name: DBHelper

package com.example.sqllitecruddemo;

import android.content.ContentValues;

import android.content.Context;

import android.database.Cursor;

import android.database.sqlite.SQLiteDatabase;

================== PAGE BREAK ==================

PAGE 133
import android.database.sqlite.SQLiteOpenHelper;

public class DBHelper extends SQLiteOpenHelper {

  public DBHelper(Context context) {

       super(context, "StudentDB", null, 1);

  }

  @Override

  public void onCreate(SQLiteDatabase db) {

       db.execSQL("CREATE TABLE student(name TEXT)");

  }

  @Override

  public void onUpgrade(SQLiteDatabase db, int oldVersion, int newVersion) {

================== PAGE BREAK ==================

PAGE 134
            db.execSQL("DROP TABLE IF EXISTS student");

     onCreate(db);

}

// Insert

public void insertData(String name) {

     SQLiteDatabase db = this.getWritableDatabase();

     ContentValues values = new ContentValues();

     values.put("name", name);

     db.insert("student", null, values);

}

// View

public String viewData() {

================== PAGE BREAK ==================

PAGE 135
    SQLiteDatabase db = this.getReadableDatabase();

    Cursor cursor = db.rawQuery("SELECT * FROM student", null);

    StringBuilder data = new StringBuilder();

    while (cursor.moveToNext()) {

            data.append(cursor.getString(0)).append("\n");

    }

    cursor.close();

    return data.toString();

}

// Update

================== PAGE BREAK ==================

PAGE 136
public void updateData(String oldName, String newName) {

    SQLiteDatabase db = this.getWritableDatabase();

    ContentValues values = new ContentValues();

    values.put("name", newName);

    db.update(

            "student",

            values,

            "name=?",

            new String[]{oldName}

    );

}

// Delete

public void deleteData(String name) {

    SQLiteDatabase db = this.getWritableDatabase();

================== PAGE BREAK ==================

PAGE 137
     db.delete(

              "student",

              "name=?",

        new String[]{name}

         );

     }

}

MainActivity.java

package com.example.sqllitecruddemo;

import android.os.Bundle;

import android.widget.Button;

import android.widget.EditText;

import android.widget.TextView;
import android.widget.Toast;

import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {
  private EditText etName, etNewName;

    private TextView txtResult;
    private DBHelper dbHelper;

    @Override

================== PAGE BREAK ==================

PAGE 138
protected void onCreate(Bundle savedInstanceState) {

  super.onCreate(savedInstanceState);

  setContentView(R.layout.activity_main);

  etName = findViewById(R.id.etName);
  etNewName = findViewById(R.id.etNewName);

  txtResult = findViewById(R.id.txtResult);

  Button btnInsert = findViewById(R.id.btnInsert);

  Button btnView = findViewById(R.id.btnView);

  Button btnUpdate = findViewById(R.id.btnUpdate);
  Button btnDelete = findViewById(R.id.btnDelete);

  dbHelper = new DBHelper(this);

  btnInsert.setOnClickListener(v -> {

        String name = etName.getText().toString().trim();

        if (name.isEmpty()) { showMessage("Enter a name first"); return; }
        dbHelper.insertData(name);

        showMessage("Data inserted");
        etName.setText("");

  });

  btnView.setOnClickListener(v -> {

        String data = dbHelper.viewData();

        txtResult.setText(data.isEmpty() ? "No records found" : data);
  });

  btnUpdate.setOnClickListener(v -> {

        String oldName = etName.getText().toString().trim();

        String newName = etNewName.getText().toString().trim();

        if (oldName.isEmpty() || newName.isEmpty()) { showMessage("Enter old and new names"); return; }
        dbHelper.updateData(oldName, newName);

        showMessage("Update completed for matching name(s)");
  });

  btnDelete.setOnClickListener(v -> {
     String name = etName.getText().toString().trim();

        if (name.isEmpty()) { showMessage("Enter a name to delete"); return; }
        dbHelper.deleteData(name);

        showMessage("Delete completed for matching name(s)");

================== PAGE BREAK ==================

PAGE 139
        });

    }

    private void showMessage(String message) {

        Toast.makeText(this, message, Toast.LENGTH_SHORT).show();
    }

}

Module 2 â€“ Practical 11
Develop an Android application integrating SQLite with ListView or RecyclerView.

â† Back to Index

11. Develop an Android application integrating SQLite with ListView or RecyclerView.

Project Name : SQLiteCRUDDemo
activity_main.xml

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

xmlns:android="http://schemas.android.com/apk/res/android"

    android:layout_width="match_parent"

    android:layout_height="match_parent"

    android:orientation="vertical"

    android:padding="20dp">

================== PAGE BREAK ==================

PAGE 140
<EditText

    android:id="@+id/etName"

    android:layout_width="match_parent"

    android:layout_height="wrap_content"

    android:hint="Enter Name" />

<Button

    android:id="@+id/btnInsert"

    android:layout_width="match_parent"

    android:layout_height="wrap_content"

    android:text="Insert" />

<Button

    android:id="@+id/btnView"

    android:layout_width="match_parent"

    android:layout_height="wrap_content"

    android:text="View Data" />

<ListView

    android:id="@+id/listView"

    android:layout_width="match_parent"

================== PAGE BREAK ==================

PAGE 141
      android:layout_height="wrap_content" />

</LinearLayout>

Create New Java Class in Package Folder

Name as: DBHelper

package com.example.sqlitecruddemo;

import android.content.ContentValues;

import android.content.Context;

import android.database.Cursor;

import android.database.sqlite.SQLiteDatabase;

import android.database.sqlite.SQLiteOpenHelper;

import java.util.ArrayList;

================== PAGE BREAK ==================

PAGE 142
public class DBHelper extends SQLiteOpenHelper {

    public DBHelper(Context context) {

    super(context, "StudentDB", null, 1);

}

@Override

public void onCreate(SQLiteDatabase db) {

    db.execSQL("CREATE TABLE student(name TEXT)");

}

@Override

public void onUpgrade(SQLiteDatabase db, int oldVersion, int newVersion) {

    // Database upgrade code goes here

}

================== PAGE BREAK ==================

PAGE 143
// Insert Data

public void insertData(String name) {

    SQLiteDatabase db = this.getWritableDatabase();

    ContentValues values = new ContentValues();

    values.put("name", name);

    db.insert("student", null, values);

}

// Get All Data

public ArrayList<String> getData() {

         ArrayList<String> list = new ArrayList<>();

         SQLiteDatabase db = this.getReadableDatabase();

================== PAGE BREAK ==================

PAGE 144
        Cursor cursor = db.rawQuery("SELECT name FROM student", null);

        while (cursor.moveToNext()) {

            list.add(cursor.getString(0));

        }

        cursor.close();

        return list;

    }

}

MainActivity.java

================== PAGE BREAK ==================

PAGE 145
package com.example.sqlitecruddemo;

import android.os.Bundle;

import android.widget.ArrayAdapter;

import android.widget.Button;

import android.widget.EditText;

import android.widget.ListView;

import android.widget.Toast;

import androidx.appcompat.app.AppCompatActivity;

import java.util.ArrayList;

public class MainActivity extends AppCompatActivity {

 EditText etName;

 Button btnInsert, btnView;

================== PAGE BREAK ==================

PAGE 146
ListView listView;

DBHelper dbHelper;

@Override

protected void onCreate(Bundle savedInstanceState) {

     super.onCreate(savedInstanceState);

     setContentView(R.layout.activity_main);

     etName = findViewById(R.id.etName);

     btnInsert = findViewById(R.id.btnInsert);

     btnView = findViewById(R.id.btnView);

     listView = findViewById(R.id.listView);

================== PAGE BREAK ==================

PAGE 147
      dbHelper = new DBHelper(this);

// Insert Data

btnInsert.setOnClickListener(v -> {

      String name = etName.getText().toString();

      dbHelper.insertData(name);

      Toast.makeText(

        this,

        "Data Inserted",

        Toast.LENGTH_SHORT

      ).show();

      etName.setText("");

});

================== PAGE BREAK ==================

PAGE 148
// View Data

btnView.setOnClickListener(v -> {

        ArrayList<String> list = dbHelper.getData();

        ArrayAdapter<String> adapter = new ArrayAdapter<>(

               this,

               android.R.layout.simple_list_item_1,

               list

        );

                listView.setAdapter(adapter);

         });

    }

}

================== PAGE BREAK ==================

PAGE 149
Module 2 â€“ Practical 12
Develop an Android application to fetch and parse JSON data from a web

â† Back to Index

12. Develop an Android application to fetch and parse JSON data from a web

PROJECTNAME: JSONDEMO

Add Internet Permission.
AndroidManifest.xml
Add following above: <application> tag
<uses-permission android:name="android.permission.INTERNET"/>

activity_main.xml

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

 xmlns:android="http://schemas.android.com/apk/res/android"

   android:layout_width="match_parent"

   android:layout_height="match_parent"

   android:orientation="vertical"

   android:padding="20dp">

================== PAGE BREAK ==================

PAGE 150
  <Button

      android:id="@+id/btnFetch"

      android:layout_width="match_parent"

      android:layout_height="wrap_content"

      android:text="Fetch JSON Data" />

  <TextView

      android:id="@+id/txtResult"

      android:layout_width="match_parent"

      android:layout_height="wrap_content"

      android:layout_marginTop="20dp"

      android:textSize="18sp"

      android:textColor="#000000" />

</LinearLayout>

================== PAGE BREAK ==================

PAGE 151
MainActivity.java

package com.example.jsondemo;

import android.os.Bundle;

import android.widget.Button;

import android.widget.TextView;

import java.io.BufferedReader;

import java.io.InputStreamReader;

import java.net.HttpURLConnection;

import java.net.URL;

import org.json.JSONObject;

import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

 Button btnFetch;

 TextView txtResult;

================== PAGE BREAK ==================

PAGE 152
@Override

protected void onCreate(Bundle savedInstanceState) {

    super.onCreate(savedInstanceState);

    setContentView(R.layout.activity_main);

    btnFetch = findViewById(R.id.btnFetch);

    txtResult = findViewById(R.id.txtResult);

    btnFetch.setOnClickListener(v -> {

            fetchData();

    });

}

private void fetchData() {

================== PAGE BREAK ==================

PAGE 153
      new Thread(() -> {

          try {

              // Web Service URL

               URL url = new
URL("https://jsonplaceholder.typicode.com/posts/1");

              HttpURLConnection connection =

        (HttpURLConnection) url.openConnection();

              connection.setRequestMethod("GET");

================== PAGE BREAK ==================

PAGE 154
        BufferedReader reader = new BufferedReader(new
InputStreamReader(

        connection.getInputStream()

         )

);

StringBuilder result = new StringBuilder();

String line;

while ((line = reader.readLine()) != null) {

     result.append(line);

}

================== PAGE BREAK ==================

PAGE 155
reader.close();

// JSON Parsing

JSONObject jsonObject =

         new JSONObject(result.toString());

String title =

         jsonObject.getString("title");

    String body =

        jsonObject.getString("body");

    // Display Data

    runOnUiThread(() -> {

            txtResult.setText(

        "Title: " + title +

================== PAGE BREAK ==================

PAGE 156
        "\n\nBody: " + body

            );

    });

    connection.disconnect();

} catch (Exception e) {

    e.printStackTrace();

    runOnUiThread(() -> {

            txtResult.setText(

        "Error: " + e.getMessage()

            );

    });

}

          }).start();

    }

}

================== PAGE BREAK ==================

PAGE 157
https://jsonplaceholder.typicode.com/posts/1

================== PAGE BREAK ==================

PAGE 158
Module 2 â€“ Practical 13
Develop an Android application demonstrating Threads and Handlers for background
processing.

â† Back to Index

        Concurrency, Media and Security

13. Develop an Android application demonstrating Threads and Handlers for background
processing.

Project Name: ThreadHandlerDemo

Activity_main.xml

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

    xmlns:android="http://schemas.android.com/apk/res/android"

    android:layout_width="match_parent"

    android:layout_height="match_parent"

    android:orientation="vertical"

    android:gravity="center"

    android:padding="20dp">

    <Button

       android:id="@+id/btnStart"

       android:layout_width="wrap_content"

       android:layout_height="wrap_content"

================== PAGE BREAK ==================

PAGE 159
       android:text="Start Background Task"/>

    <TextView

       android:id="@+id/txtResult"

       android:layout_width="wrap_content"

       android:layout_height="wrap_content"

       android:textSize="22sp"

       android:paddingTop="20dp"/></LinearLayout>

MainActivity.java

package com.example.threadhandlerdemo;

import android.os.Bundle;

import android.os.Handler;

import android.os.Looper;

import android.widget.Button;

import android.widget.TextView;

import androidx.appcompat.app.AppCompatActivity;

================== PAGE BREAK ==================

PAGE 160
public class MainActivity extends AppCompatActivity {

   Button btnStart;

   TextView txtResult;

   Handler handler = new Handler(Looper.getMainLooper());

   @Override

   protected void onCreate(Bundle savedInstanceState) {

       super.onCreate(savedInstanceState);

       setContentView(R.layout.activity_main);

       btnStart = findViewById(R.id.btnStart);

       txtResult = findViewById(R.id.txtResult);

       btnStart.setOnClickListener(v -> {

================== PAGE BREAK ==================

PAGE 161
// Background Thread

Thread thread = new Thread(() -> {

      try {

              // Simulate Background Work

              Thread.sleep(3000);

      } catch (Exception e) {

              e.printStackTrace();

      }

      // Update UI using Handler

      handler.post(() -> {

              txtResult.setText("Background Task Completed");

      });

});

================== PAGE BREAK ==================

PAGE 162
              thread.start();

        });

    }

}

================== PAGE BREAK ==================

PAGE 163
Module 2 â€“ Practical 15
Develop an Android application implementing Runtime Permissions and security handling
in AndroidManifest.xml.

â† Back to Index

15. Develop an Android application implementing Runtime Permissions and security
handling in AndroidManifest.xml

Project Name:PermissionDemo

Add Permission in AndroidManifest.xml.
Open:
AndroidManifest.xml
Add below code lines above: <application> tag
<uses-permission android:name="android.permission.CAMERA"/>
<uses-feature android:name="android.hardware.camera"
android:required="false" />

activity_main.xml
<?xml version="1.0" encoding="utf-8"?>

<LinearLayout

 xmlns:android="http://schemas.android.com/apk/res/android"

   android:layout_width="match_parent"

   android:layout_height="match_parent"

   android:gravity="center">

   <Button

       android:id="@+id/btnPermission"

       android:layout_width="wrap_content"

================== PAGE BREAK ==================

PAGE 164
       android:layout_height="wrap_content"

        android:text="Request Camera Permission"/>

</LinearLayout>

MainActivity.java

package com.example.permissiondemo;

import android.content.pm.PackageManager;

import android.os.Bundle;

import android.widget.Button;

import android.widget.Toast;

import androidx.appcompat.app.AppCompatActivity;

import androidx.core.app.ActivityCompat;

import androidx.core.content.ContextCompat;

public class MainActivity extends AppCompatActivity {

================== PAGE BREAK ==================

PAGE 165
    Button btnPermission;

     @Override

     protected void onCreate(Bundle savedInstanceState) {

            super.onCreate(savedInstanceState);

            setContentView(R.layout.activity_main);

            btnPermission = findViewById(R.id.btnPermission);

      btnPermission.setOnClickListener(v -> {

              checkPermission();

      });

}

private void checkPermission() {

================== PAGE BREAK ==================

PAGE 166
// Check if Camera permission is already granted

if (ContextCompat.checkSelfPermission(

           this,

           android.Manifest.permission.CAMERA

) == PackageManager.PERMISSION_GRANTED) {

      Toast.makeText(

               this,

               "Permission Already Granted",

               Toast.LENGTH_SHORT

      ).show();

} else {

      // Request Camera permission

      ActivityCompat.requestPermissions(

================== PAGE BREAK ==================

PAGE 167
        this,

        new String[]{

        android.Manifest.permission.CAMERA

        },

        1

            );

      }

}

// Permission Result

@Override

public void onRequestPermissionsResult(

            int requestCode,

            String[] permissions,

            int[] grantResults

){

      super.onRequestPermissionsResult(

        requestCode,

        permissions,

================== PAGE BREAK ==================

PAGE 168
         grantResults

);

if (requestCode == 1) {

     if (grantResults.length > 0

             && grantResults[0] == PackageManager.PERMISSION_GRANTED) {

         Toast.makeText(

        this,

        "Permission Granted",

        Toast.LENGTH_SHORT

         ).show();

     } else {

================== PAGE BREAK ==================

PAGE 169
                Toast.makeText(

        this,

        "Permission Denied",

        Toast.LENGTH_SHORT

                ).show();

            }

        }

    }

}

================== PAGE BREAK ==================

PAGE 170
Source Coverage Note

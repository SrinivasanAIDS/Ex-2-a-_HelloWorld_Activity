

# Ex.No:1 Implementation of a Hello world Activity using all lifecycles methods using Android Studio.


## AIM:
To create Hello world Activity using all lifecycles methods to display messages using android studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min. required Artic Fox)


## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.



## Program:
 ```
/*
Program to print the text “Hello World”.
Developed by: Srinivasan S
Registeration Number : 212220230048
*/
```

## MainActivity.java:
```java
package com.example.myapplication;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast t2= Toast.makeText(getApplicationContext(),"onCreate Executed",Toast.LENGTH_LONG);
        t2.show();
    }
    protected void onStart(){
        super.onStart();
        Toast t2= Toast.makeText(getApplicationContext(),"onStart Executed",Toast.LENGTH_LONG);
        t2.show();
    }
    protected void onResume(){
        super.onResume();
        Toast t2= Toast.makeText(getApplicationContext(),"onResume Executed",Toast.LENGTH_LONG);
        t2.show();
    }
    protected void onPause(){
        super.onPause();
        Toast t2= Toast.makeText(getApplicationContext(),"onPause Executed",Toast.LENGTH_LONG);
        t2.show();
    }
    protected void onRestart(){
        super.onRestart();
        Toast t2= Toast.makeText(getApplicationContext(),"onRestart Executed",Toast.LENGTH_LONG);
        t2.show();
    }
    protected void onStop(){
        super.onStop();
        Toast t2= Toast.makeText(getApplicationContext(),"onStop Executed",Toast.LENGTH_LONG);
        t2.show();
    }
    protected void onDestroy(){
        super.onDestroy();
        Toast t2= Toast.makeText(getApplicationContext(),"onDestory Executed",Toast.LENGTH_LONG);
        t2.show();
    }
}
```

## activity_main.xml:
```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
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

</androidx.constraintlayout.widget.ConstraintLayout>
```

## Output:
![image](https://github.com/SrinivasanAIDS/Ex-2-a-_HelloWorld_Activity/assets/103049243/b2bfd0c5-4977-48a6-abb3-7c16264db73b)

## Result:
Thus a program to implement the various life cycles of an activity is written and successfully executed using Android Studio.

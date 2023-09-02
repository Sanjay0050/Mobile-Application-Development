# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Hello World”.
Developed by: sanjay P
Registeration Number :212221220047
*/
```
## MainActivity.Java:
```
package com.example.helloworld;
import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle; import android.widget.Toast;

public class MainActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast t = Toast.makeText(getApplicationContext(),"onCreate Called",Toast.LENGTH_LONG);
        t.show();
    }

    protected void onStart(){
        super.onStart();
        Toast t = Toast.makeText(getApplicationContext(),"onStart Called",Toast.LENGTH_LONG);
        t.show();
    }

    protected void onRestart(){
        super.onRestart();
        Toast t = Toast.makeText(getApplicationContext(),"onRestart Called",Toast.LENGTH_LONG);
        t.show();
    }

    protected void onPause(){
        super.onPause();
        Toast t = Toast.makeText(getApplicationContext(),"onPause Called",Toast.LENGTH_LONG);
        t.show();
    }

    protected void onResume(){
        super.onResume();
        Toast t = Toast.makeText(getApplicationContext(),"onResume Called",Toast.LENGTH_LONG);
        t.show();
    }

    protected void onStop(){
        super.onStop();
        Toast t = Toast.makeText(getApplicationContext(),"onStop Called",Toast.LENGTH_LONG);
        t.show();
    }

    protected void onDestroy(){
        super.onDestroy();
        Toast t = Toast.makeText(getApplicationContext(),"onDestroy Called",Toast.LENGTH_LONG);
        t.show();

    }
}
```
## Activity_main.xml:
```
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
    <TextView
        android:id="@+id/body"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginBottom="356dp"
        android:text="HELLO WORLD"
        android:textSize="20sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.498"
        app:layout_constraintStart_toStartOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>
```

## OUTPUT
![Screenshot (20)](https://github.com/suryacse05/Mobile-Application-Development/assets/108233895/a52d9a3a-876a-4cba-a1e0-6f0e54b1cfc2)

![Screenshot (21)](https://github.com/suryacse05/Mobile-Application-Development/assets/108233895/003b01a2-1b30-4ea6-ba08-fe4d0ea57d12)

![Screenshot (22)](https://github.com/suryacse05/Mobile-Application-Development/assets/108233895/d775614d-1860-4f32-a493-de7c1520189a)


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.

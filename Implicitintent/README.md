# Ex.No:3 Develop program to create a text field and a button “Navigate”. When you enter “www.google.com” and press navigate button it should open google page using Implicit Intents.


## AIM:

To create a navigate button using Implicit Intent to display the google page using Android Studio.

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
Program to print the text “Implicitintent”.
Developed by: Sanjay
Registeration Number : 212221220047
*/
```
```
/*
MAINACTIVITY.JAVA :-
package com.example.ex3;
import androidx.appcompat.app.AppCompatActivity;
import android.content.Intent;
import android.net.Uri;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
public class MainActivity extends AppCompatActivity {
 Button button;
 EditText e1;
 @Override
 protected void onCreate(Bundle savedInstanceState) {
 super.onCreate(savedInstanceState);
 setContentView(R.layout.activity_main);
 button = findViewById(R.id.button);
 e1 = findViewById(R.id.E1);
 button.setOnClickListener(view -> {
 String url = e1.getText().toString();
 Intent i1 = new Intent(Intent.ACTION_VIEW, Uri.parse(url));
 startActivity(i1);
 });
 }
}


ACTIVITYMAIN.XML :-

<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
 xmlns:android="http://schemas.android.com/apk/res/android"
 xmlns:app="http://schemas.android.com/apk/res-auto"
 xmlns:tools="http://schemas.android.com/tools"
 android:layout_width="match_parent"
 android:layout_height="match_parent"
 tools:context=".MainActivity">
 <TextView
 android:id="@+id/textView"
 android:layout_width="wrap_content"
 android:layout_height="wrap_content"
 android:layout_marginStart="44dp"
 android:layout_marginTop="52dp"
 android:text="Enter link:"
 android:textSize="26sp"
 app:layout_constraintBottom_toTopOf="@+id/E1"
 app:layout_constraintStart_toStartOf="parent"
 app:layout_constraintTop_toTopOf="parent"
 app:layout_constraintVertical_bias="0.693"
 tools:ignore="ExtraText" />
 <EditText
 android:id="@+id/E1"
 android:layout_width="217dp"
 android:layout_height="85dp"
 android:layout_marginTop="144dp"
 android:ems="10"
 android:inputType="textPersonName"
 android:text="link"
 android:textColor="#2196F3"
 app:layout_constraintBottom_toTopOf="@+id/button"
 app:layout_constraintEnd_toEndOf="parent"
 app:layout_constraintHorizontal_bias="0.552"
 app:layout_constraintStart_toStartOf="parent"
 app:layout_constraintTop_toTopOf="parent" />
 <Button
 android:id="@+id/button"
 android:layout_width="wrap_content"
 android:layout_height="wrap_content"
 android:layout_marginBottom="248dp"
 android:text="GO"
 app:backgroundTint="#4CAF50"
 app:layout_constraintBottom_toBottomOf="parent"
 app:layout_constraintEnd_toEndOf="parent"
 app:layout_constraintHorizontal_bias="0.547"
 app:layout_constraintStart_toStartOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>

*/
```
## Layout:
![ex3-1](https://github.com/KGSatheeshKumar/Mobile-Application-Development/assets/128453421/442c477c-787e-4f93-9377-d7163e34fb4d)
![ex3-2](https://github.com/KGSatheeshKumar/Mobile-Application-Development/assets/128453421/c2cb1628-a291-44ae-bc55-31bd30e08e00)
![ex3-3](https://github.com/KGSatheeshKumar/Mobile-Application-Development/assets/128453421/48decfdb-6b1b-4570-9d65-0f3a83067c8d)
## Output

![a1](https://github.com/KGSatheeshKumar/Mobile-Application-Development/assets/128453421/e8fb5c6b-5c6a-4055-8470-c0dce6c7afb8)
![a2](https://github.com/KGSatheeshKumar/Mobile-Application-Development/assets/128453421/0f475948-91f6-4bd1-8934-6aa08b46d4df)

## RESULT:
Thus a Simple Android Application create a navigate button using Implicit Intent to display the google page using Android Studio is developed and executed successfully.

# Ex.No:10 To create a option menu to display menu items.


## AIM:

To create a option menu to display menu items using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:



## PROGRAM:
```
/*
Program to print the text “optionmenu”.
Developed by: Sanjay P
Registeration Number : 212221220047
*/
```

**XML CODE:**

    <?xml version="1.0" encoding="utf-8"?>
    <androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <ImageView
        android:id="@+id/imageView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:src="@drawable/amgus"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        tools:srcCompat="@tools:sample/avatars" />
    </androidx.constraintlayout.widget.ConstraintLayout>
    
**OPTION XML CODE:**

    <?xml version="1.0" encoding="utf-8"?>
    <menu xmlns:android="http://schemas.android.com/apk/res/android">
    <item android:title="PRIME 1" />
    <item android:title="PRIME 2" />
    <item android:title="PRIME 3" />
    </menu>
**MAIN ACTIVITY CODE:**

      package com.example.menuapp;

    import androidx.appcompat.app.AppCompatActivity;

    import android.os.Bundle;
    import android.view.Menu;
    import android.view.MenuInflater;

    public class MainActivity extends AppCompatActivity {
     @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
    @Override
    public boolean onCreateOptionsMenu(Menu menu) {
        MenuInflater m = getMenuInflater();
        m.inflate(R.menu.option,menu);
        return true;
    }
    }

## OUTPUT

![Xml](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/b7cc1ff6-2b96-469d-aa49-e1d5a95295ca) <br>
![Main](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/25badaf2-006c-4716-a599-cb60479fedf8) <br>
![mad1](https://github.com/KGSatheeshKumar/Mobile-Application-Development/assets/128453421/9b1e3469-68c4-4442-87f6-f496813024f4)

<br><br><br><br><br><br><br><br><br><br><br><br>




## RESULT
Thus a Simple Android Application to create a option menu to display menu items using Android Studio is developed and executed successfully.

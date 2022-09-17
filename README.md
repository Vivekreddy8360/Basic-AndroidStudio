# Basic-AndroidStudio
## Program:
```
Developed by: M.vivek reddy
Rgistration Number: 212221240030
```
## MainActiviity.java
```
package com.example.activitylifecycle;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast=Toast.makeText(getApplicationContext(),"OnCreate Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStart(){
        super.onStart();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStart Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onResume(){
        super.onResume();
        Toast toast=Toast.makeText(getApplicationContext(),"OnResume Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onPause(){
        super.onPause();
        Toast toast=Toast.makeText(getApplicationContext(),"OnPause Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStop(){
        super.onStop();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStop Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onDestroy(){
        super.onDestroy();
        Toast toast=Toast.makeText(getApplicationContext(),"OnDestroy Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onRestart(){
        super.onRestart();
        Toast toast=Toast.makeText(getApplicationContext(),"OnRestart Executed",Toast.LENGTH_LONG);
        toast.show();
    }
```
## activity_main.xml
```
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
## Output

![activity1](https://user-images.githubusercontent.com/94525701/190870148-6ff7ffe9-3499-41cc-bea5-39f50edf6594.jpg)
![activity2](https://user-images.githubusercontent.com/94525701/190870160-533f5508-15db-4764-bd0a-bd0e7869723b.jpg)
![activityxml3](https://user-images.githubusercontent.com/94525701/190870167-5954b9ed-ea67-4088-b622-8b9e7cc4cd70.jpg)
![helloworld](https://user-images.githubusercontent.com/94525701/190870177-a0efd566-ccb1-4c06-b32a-db8bccf3eddb.jpeg)
![activityoncreate](https://user-images.githubusercontent.com/94525701/190870185-aca3a02e-91e3-4827-97d2-62e873c0397e.jpeg)
![activitiy4](https://user-images.githubusercontent.com/94525701/190870192-dce79024-ff55-4fa1-a5a7-c42ced2f523f.jpeg)
![onpause](https://user-images.githubusercontent.com/94525701/190870314-6d3860ae-dce6-4588-9479-4a733b0d7e37.jpeg)
![actresume](https://user-images.githubusercontent.com/94525701/190870297-7a9a47ee-13de-48ea-9776-cfa8acade5dd.jpeg)
![onstop](https://user-images.githubusercontent.com/94525701/190870362-405c72b3-8e5e-426a-85d3-8126825bf4c4.jpeg)




## Result
Therefore a program is return to develop a program to detect the various life cycles of an activity. The program is successfully executed.


# Ex.No:2a Implicit Intent

Develop program to create a text field and a button “Navigate”. When you enter “www.google.com” and press navigate button it should open google page using Implicit Intents.


## AIM:

To create a layout,click button,open google page using Implicit Intents in Android Studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min. required Artic Fox)

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as ImplicitIntent and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: open google page using Implicit Intents in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Implicit Intent”.
Developed by:Vivek Reddy
Registeration Number :212221240030
*/
```
### MainActivity.java
```
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/txtView1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Enter the website link"

        android:layout_centerHorizontal="true"
        android:layout_marginTop="300dp"
        android:textSize="25sp"
        android:textStyle="bold"
        />
    <EditText
        android:id="@+id/edit1"
        android:layout_height="40dp"
        android:layout_width="250dp"
        android:hint="Enter here"
        android:layout_below="@+id/txtView1"
        android:layout_marginTop="20dp"
        android:layout_centerHorizontal="true"
        />
    <Button
        android:id="@+id/Button1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Search"
        android:layout_below="@+id/edit1"
        android:layout_centerHorizontal="true"
        android:layout_marginTop="20dp"/>

</RelativeLayout>
```
## activity_main.xml
```
package com.example.exp2;

import androidx.appcompat.app.AppCompatActivity;

import android.content.Intent;
import android.os.Bundle;
import android.widget.Button;
import android.widget.EditText;
import android.net.Uri;

public class MainActivity extends AppCompatActivity {
        EditText edit1;
        Button Button1;

        @Override
        protected void onCreate(Bundle savedInstanceState) {
                super.onCreate(savedInstanceState);
                setContentView(R.layout.activity_main);
                edit1 = findViewById(R.id.edit1);
                Button1 = findViewById(R.id.Button1);

                Button1.setOnClickListener(view ->{
                        String  url = edit1.getText().toString();
                        Intent intent = new Intent(Intent.ACTION_VIEW,Uri.parse(url));
                        startActivity(intent);
                });

        }
}
```

## OUTPUT:
![vivek2a](https://user-images.githubusercontent.com/94525701/190564790-83d51522-40a5-4c7d-a844-b5463e330def.png)

![vivek2a 1](https://user-images.githubusercontent.com/94525701/190564801-c45e3cc0-7dfb-4b9c-87a4-518cdc3b4cd8.png)

## RESULT
Thus a Simple Android Application to open google page using Implicit Intents using Android Studio is developed and executed successfully.

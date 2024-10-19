## WORKSHOP ----SUMMATION OF TWO NUMBERS USING ANDROID STUDIO.


## AIM:
Summation of two numbers using Android Studio


## EQUIPMENTS REQUIRED:

Android Studio(Min. required Artic Fox)


## ALGORITHM:

Step 1: Begin the program. 

Step 2: Prompt the user to input the first number. 

Step 3: Prompt the user to input the second number. 

Step 4: Check if both inputs are valid numbers. 

Step 5: If any input is invalid, display an error message and return to step 2. 

Step 6: Add the two numbers together to find their sum. 

Step 7: Display the sum to the user. 

Step 8: End the program

## Program:
 ```
/*
Program to implement a Hello world Activity using all lifecycles methods using Android Studio .
Developed by: HIRUTHIK SUDHAKAR
RegisterNumber:  212223240054
*/
```

## MainActivity.java:

```java
package com.example.myapplication;

import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import android.widget.TextView;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        final EditText num1 = (EditText) findViewById(R.id.num1);
        final EditText num2 = (EditText) findViewById(R.id.num2);
        final TextView result = (TextView) findViewById(R.id.result);
        Button addButton = (Button) findViewById(R.id.addButton);

        addButton.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                int sum = Integer.parseInt(num1.getText().toString()) + Integer.parseInt(num2.getText().toString());
                result.setText(String.valueOf(sum));
            }
        });
    }
}
```




## activity_main.xml:

```xml
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <EditText
        android:id="@+id/num1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:inputType="number"
        android:hint="Enter first number"/>

    <EditText
        android:id="@+id/num2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:inputType="number"
        android:hint="Enter second number"
        android:layout_below="@id/num1"/>

    <Button
        android:id="@+id/addButton"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Add"
        android:layout_below="@id/num2"/>

    <TextView
        android:id="@+id/result"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_below="@id/addButton"
        android:text="Result will be displayed here"/>

</RelativeLayout>
```

## Output:

<img width="540" alt="328074222-fb3d6fa3-0fcc-4b85-bba9-bf3d43656454" src="https://github.com/user-attachments/assets/d3bb6c1b-b79a-4766-a791-fe47bee1857e">



## Result:

Thus successfully we have added two numbers using android studio.


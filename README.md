## EX:NO:05:Develop a program to create a simple calculator using android studio.
## Aim:
To create and design an android application for a simple calculator using android studio.
## EQUIPMENTS REQUIRED:
Android Studio(Latest Version)
## ALGORITHM:
Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as smsintent and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6:Display details give in MainActivity file.

Step 7: Save and run the application.
## PROGRAM:
Program to create and design an android application simple calculator using Intent.
### Developed by: Ramkumar S
### Registration Number : 212223220085

## activity_main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@color/white"
    android:orientation="vertical"
    android:padding="16dp"
    tools:context=".MainActivity">

    <!-- Input Field -->

    <!-- Result Display -->

    <!-- Buttons Grid -->

    <EditText
        android:id="@+id/editText2"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:backgroundTint="@color/black"
        android:gravity="center"
        android:hint="Enter Value"
        android:inputType="text"
        android:padding="10dp"
        android:textColor="@color/black"
        android:textSize="24sp"
        android:translationY="250dp"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/resultText"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:gravity="center"
        android:text="Result"
        android:textColor="@color/black"
        android:textSize="22sp"
        android:translationY="260dp"
        app:layout_constraintTop_toBottomOf="@+id/editText2"
        tools:layout_editor_absoluteX="47dp" />

    <GridLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_gravity="center"
        android:alignmentMode="alignMargins"
        android:columnCount="4"
        android:rowCount="5"
        android:rowOrderPreserved="false"
        android:translationY="280dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/resultText"
        app:layout_constraintVertical_bias="0.13">

        <!-- Row 1 -->
        <Button
            android:id="@+id/num7"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_columnWeight="1"
            android:layout_margin="4dp"
            android:backgroundTint="#E8F5E9"
            android:text="7"
            android:textColor="@color/black"
            android:textSize="20sp" />

        <Button
            android:id="@+id/num8"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_columnWeight="1"
            android:layout_margin="4dp"
            android:backgroundTint="#E8F5E9"
            android:text="8"
            android:textColor="@color/black"
            android:textSize="20sp" />

        <Button
            android:id="@+id/num9"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_columnWeight="1"
            android:layout_margin="4dp"
            android:backgroundTint="#E8F5E9"
            android:text="9"
            android:textColor="@color/black"
            android:textSize="20sp" />

        <Button
            android:id="@+id/div"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_columnWeight="1"
            android:layout_margin="4dp"
            android:backgroundTint="#E8F5E9"
            android:text="/"
            android:textColor="@color/black"
            android:textSize="20sp" />

        <!-- Row 2 -->
        <Button
            android:id="@+id/num4"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_columnWeight="1"
            android:layout_margin="4dp"
            android:backgroundTint="#E8F5E9"
            android:text="4"
            android:textColor="@color/black"
            android:textSize="20sp" />

        <Button
            android:id="@+id/num5"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_columnWeight="1"
            android:layout_margin="4dp"
            android:backgroundTint="#E8F5E9"
            android:text="5"
            android:textColor="@color/black"
            android:textSize="20sp" />

        <Button
            android:id="@+id/num6"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_columnWeight="1"
            android:layout_margin="4dp"
            android:backgroundTint="#E8F5E9"
            android:text="6"
            android:textColor="@color/black"
            android:textSize="20sp" />

        <Button
            android:id="@+id/mul"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_columnWeight="1"
            android:layout_margin="4dp"
            android:backgroundTint="#E8F5E9"
            android:text="×"
            android:textColor="@color/black"
            android:textSize="20sp" />

        <!-- Row 3 -->
        <Button
            android:id="@+id/num1"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_columnWeight="1"
            android:layout_margin="4dp"
            android:backgroundTint="#E8F5E9"
            android:text="1"
            android:textColor="@color/black"
            android:textSize="20sp" />

        <Button
            android:id="@+id/num2"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_columnWeight="1"
            android:layout_margin="4dp"
            android:backgroundTint="#E8F5E9"
            android:text="2"
            android:textColor="@color/black"
            android:textSize="20sp" />

        <Button
            android:id="@+id/num3"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_columnWeight="1"
            android:layout_margin="4dp"
            android:backgroundTint="#E8F5E9"
            android:text="3"
            android:textColor="@color/black"
            android:textSize="20sp" />

        <Button
            android:id="@+id/sub"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_columnWeight="1"
            android:layout_margin="4dp"
            android:backgroundTint="#E8F5E9"
            android:text="−"
            android:textColor="@color/black"
            android:textSize="20sp" />

        <!-- Row 4 -->
        <Button
            android:id="@+id/num0"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_columnWeight="1"
            android:layout_margin="4dp"
            android:backgroundTint="#E8F5E9"
            android:text="0"
            android:textColor="@color/black"
            android:textSize="20sp" />

        <Button
            android:id="@+id/dot"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_columnWeight="1"
            android:layout_margin="4dp"
            android:backgroundTint="#E8F5E9"
            android:text="."
            android:textColor="@color/black"
            android:textSize="20sp" />

        <Button
            android:id="@+id/submit"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_columnWeight="1"
            android:layout_margin="4dp"
            android:backgroundTint="#E8F5E9"
            android:text="="
            android:textColor="@color/black"
            android:textSize="20sp" />

        <Button
            android:id="@+id/add"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_columnWeight="1"
            android:layout_margin="4dp"
            android:backgroundTint="#E8F5E9"
            android:text="+"
            android:textColor="@color/black"
            android:textSize="20sp" />

        <!-- Row 5 (Clear button) -->
        <Button
            android:id="@+id/clear_text"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_columnSpan="4"
            android:layout_marginTop="8dp"
            android:backgroundTint="#2962FF"
            android:padding="10dp"
            android:text="C"
            android:textColor="@color/white"
            android:textSize="22sp" />

    </GridLayout>

</androidx.constraintlayout.widget.ConstraintLayout>
```
#MainActivity.java
```
package com.example.calculator;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Button;
import android.widget.EditText;
import android.widget.TextView;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    EditText editText;
    TextView resultText;

    Button add, sub, mul, div, equal, clear, dot;

    Button[] nums = new Button[10];

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        editText = findViewById(R.id.editText2);
        resultText = findViewById(R.id.resultText);

        add = findViewById(R.id.add);
        sub = findViewById(R.id.sub);
        mul = findViewById(R.id.mul);
        div = findViewById(R.id.div);

        equal = findViewById(R.id.submit);
        clear = findViewById(R.id.clear_text);
        dot = findViewById(R.id.dot);

        nums[0] = findViewById(R.id.num0);
        nums[1] = findViewById(R.id.num1);
        nums[2] = findViewById(R.id.num2);
        nums[3] = findViewById(R.id.num3);
        nums[4] = findViewById(R.id.num4);
        nums[5] = findViewById(R.id.num5);
        nums[6] = findViewById(R.id.num6);
        nums[7] = findViewById(R.id.num7);
        nums[8] = findViewById(R.id.num8);
        nums[9] = findViewById(R.id.num9);

        for (int i = 0; i < 10; i++) {
            int n = i;
            nums[i].setOnClickListener(v ->
                    editText.append(String.valueOf(n)));
        }

        dot.setOnClickListener(v -> {
            String text = editText.getText().toString();

            String[] parts = text.split("[+\\-*/]");
            String last = parts[parts.length - 1];

            if (!last.contains(".")) {
                editText.append(".");
            }
        });

        add.setOnClickListener(v -> addOperator("+"));
        sub.setOnClickListener(v -> addOperator("-"));
        mul.setOnClickListener(v -> addOperator("*"));
        div.setOnClickListener(v -> addOperator("/"));

        clear.setOnClickListener(v -> {
            editText.setText("");
            resultText.setText("Result");
        });

        equal.setOnClickListener(v -> calculate());
    }

    private void addOperator(String op) {

        String text = editText.getText().toString();

        if (text.isEmpty()) {
            return;
        }

        char last = text.charAt(text.length() - 1);

        if (last != '+' && last != '-' &&
                last != '*' && last != '/') {

            editText.append(op);
        }
    }

    private void calculate() {

        String exp = editText.getText().toString();

        try {

            double result = 0;

            if (exp.contains("+")) {

                String[] n = exp.split("\\+");

                result = Double.parseDouble(n[0]) +
                        Double.parseDouble(n[1]);

            } else if (exp.contains("-")) {

                String[] n = exp.split("-");

                result = Double.parseDouble(n[0]) -
                        Double.parseDouble(n[1]);

            } else if (exp.contains("*")) {

                String[] n = exp.split("\\*");

                result = Double.parseDouble(n[0]) *
                        Double.parseDouble(n[1]);

            } else if (exp.contains("/")) {

                String[] n = exp.split("/");

                double a = Double.parseDouble(n[0]);
                double b = Double.parseDouble(n[1]);

                if (b == 0) {
                    Toast.makeText(this,
                            "Cannot divide by zero",
                            Toast.LENGTH_SHORT).show();
                    return;
                }

                result = a / b;
            }

            if (result == (int) result) {
                resultText.setText("Result: " + (int) result);
            } else {
                resultText.setText("Result: " + result);
            }

        } catch (Exception e) {

            Toast.makeText(this,
                    "Invalid Expression",
                    Toast.LENGTH_SHORT).show();
        }
    }
}
```

### output

<img width="1366" height="768" alt="Screenshot 2026-11-20 090611" src="https://github.com/user-attachments/assets/f484de22-cff2-40d9-ad13-f00d12c45c00" />


<img width="1366" height="768" alt="Screenshot 2026-11-20 091138" src="https://github.com/user-attachments/assets/2bf1fe2b-36d3-49db-a25b-bb1f5d922fa0" />


<img width="1366" height="768" alt="Screenshot 2026-11-20 090712" src="https://github.com/user-attachments/assets/52a85dd2-7c45-42e1-8a62-03e5d0eb3e3c" />

## RESULT
Thus a Simple Android Application create a simple calculator using Android Studio is developed and executed successfully.

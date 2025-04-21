# external
3.Create registration page to demonstrate basics of 
widgets available in Android. 
 
A] Code: a] 
MainActivity.java: 
 
package com.example.registrationpage; 
 
import android.os.Bundle; 
import androidx.annotation.Nullable; 
import androidx.appcompat.app.AppCompatActivity; 
public class MainActivity extends AppCompatActivity { 
    @Override 
    protected void onCreate(@Nullable Bundle savedInstanceState) { 
        super.onCreate(savedInstanceState); 
        setContentView(R.layout.activity_main); 
    } 
} 

 
b] activity_main.xml: 
 
<?xml version="1.0" encoding="utf-8"?> 
<androidx.constraintlayout.widget.ConstraintLayout 
xmlns:android="http://schemas.android.com/apk/res/android" 
    xmlns:app="http://schemas.android.com/apk/res-auto" 
    xmlns:tools="http://schemas.android.com/tools" 
    android:id="@+id/main" 
    android:layout_width="match_parent" 
    android:layout_height="match_parent" 
    android:orientation="vertical" 
    tools:context=".MainActivity"> 
 
    <LinearLayout 
        android:layout_width="match_parent" 
        android:layout_height="wrap_content" 
        android:layout_gravity="center" 
        android:orientation="vertical" 
        android:padding="10dp" 
        tools:ignore="MissingConstraints"> 
        <TextView 
            android:layout_width="match_parent" 
            android:layout_height="wrap_content" 
            android:layout_marginTop="20dp" 
            android:fontFamily="serif" 
            android:gravity="center" 
            android:text="@string/registration" 
            android:textColor="#e65100" 
            android:textSize="40sp"/> 
        <LinearLayout 
            android:layout_width="match_parent" 
            android:layout_height="wrap_content" 
            android:layout_gravity="center" 
            android:orientation="vertical" 
            android:padding="2dp"> 
            <com.google.android.material.textfield.TextInputLayout 
                android:layout_width="match_parent" 
                android:layout_height="wrap_content"> 
                <com.google.android.material.textfield.TextInputEditText 
                    android:id="@+id/nm" 
                    android:layout_width="match_parent" 
                    android:layout_height="wrap_content" 
                    android:layout_marginLeft="20dp" 
                    android:layout_marginTop="2dp" 
                    android:layout_marginRight="20dp" 
                    android:hint="@string/name" 
                    android:padding="10dp" 
                    android:textColorHint="#546E7A" 
                    
tools:ignore="TextContrastCheck,TouchTargetSizeCheck,VisualLintTextFieldSize"/> 
            </com.google.android.material.textfield.TextInputLayout> 
            <com.google.android.material.textfield.TextInputLayout 
                android:layout_width="match_parent" 
                android:layout_height="wrap_content"> 
                <com.google.android.material.textfield.TextInputEditText 
                    android:id="@+id/mob" 
                    android:layout_width="match_parent" 
                    android:layout_height="wrap_content" 
                    android:layout_marginLeft="20dp" 
                    android:layout_marginRight="20dp" 
                    android:hint="Mobile" 
                    android:padding="10dp" 
                    android:textColorHint="#546E7A" 
                    
tools:ignore="HardcodedText,TextContrastCheck,TouchTargetSizeCheck,VisualLintTextField
 Size" /> 
            </com.google.android.material.textfield.TextInputLayout> 
            <com.google.android.material.textfield.TextInputLayout 
                android:layout_width="match_parent" 
                android:layout_height="wrap_content"> 
                <com.google.android.material.textfield.TextInputEditText 
                    android:id="@+id/email" 
                    android:layout_width="match_parent" 
                    android:layout_height="wrap_content" 
                    android:layout_marginLeft="20dp" 
                    android:layout_marginRight="20dp" 
                    android:hint="@string/email" 
                    android:padding="10dp" 
                    android:textColorHint="#546E7A" 
                    
tools:ignore="TextContrastCheck,TouchTargetSizeCheck,VisualLintTexize,VisualLintTextField
 Size" /> 
            </com.google.android.material.textfield.TextInputLayout> 
            <com.google.android.material.textfield.TextInputLayout 
                android:layout_width="match_parent" 
                android:layout_height="wrap_content"> 
                <com.google.android.material.textfield.TextInputEditText 
                    android:id="@+id/pass" 
                    android:layout_width="match_parent" 
                    android:layout_height="wrap_content" 
                    android:layout_marginLeft="20dp" 
                    android:layout_marginRight="20dp" 
                    android:hint="@string/password" 
                    android:inputType="textPassword" 
                    android:padding="10dp" 
                    
tools:ignore="TextContrastCheck,TouchTargetSizeCheck,VisualLintTextFieldSize"/> 
            </com.google.android.material.textfield.TextInputLayout> 
            <com.google.android.material.textfield.TextInputLayout 
                android:layout_width="match_parent" 
                android:layout_height="wrap_content"> 
                <com.google.android.material.textfield.TextInputEditText 
                    android:id="@+id/rollNo" 
                    android:layout_width="match_parent" 
                    android:layout_height="wrap_content" 
                    android:layout_marginLeft="20dp" 
                    android:layout_marginTop="2dp" 
                    android:layout_marginRight="20dp" 
                    android:hint="@string/roll_no" 
                    android:padding="10dp" 
                    
tools:ignore="TextContrastCheck,TouchTargetSizeCheck,VisualLintTextFieldSize"/> 
            </com.google.android.material.textfield.TextInputLayout> 
            <com.google.android.material.textfield.TextInputLayout 
                android:layout_width="match_parent" 
                android:layout_height="wrap_content"> 
                <com.google.android.material.textfield.TextInputEditText 
                    android:id="@+id/age" 
                    android:layout_width="match_parent" 
                    android:layout_height="wrap_content" 
                    android:layout_marginLeft="20dp" 
                    android:layout_marginTop="2dp" 
                    android:layout_marginRight="20dp" 
                    android:hint="@string/age" 
                    android:padding="10dp" 
                    android:textColorHint="#546E7A" 
 
                    
tools:ignore="TextContrastCheck,TouchTargetSizeCheck,VisualLintTextFieldSize"/> 
            </com.google.android.material.textfield.TextInputLayout> 
            <RadioGroup 
                android:id="@+id/rd_gen" 
                android:layout_width="match_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginLeft="10dp" 
                android:layout_marginTop="10dp" 
                android:layout_marginRight="10dp" 
                android:orientation="horizontal"> 
                <RadioButton 
                    android:id="@+id/right_male" 
                    android:layout_width="wrap_content" 
                    android:layout_height="wrap_content" 
                    android:layout_marginLeft="50dp" 
                    android:gravity="center" 
                    android:text="@string/male" 
                    android:textSize="20sp" 
                    tools:ignore="RtlHardcoded" /> 
 
                <RadioButton 
                    android:id="@+id/right_female" 
                    android:layout_width="wrap_content" 
                    android:layout_height="wrap_content" 
                    android:layout_marginStart="20dp" 
                    android:text="@string/female" 
                    android:textSize="20sp" 
                    tools:ignore="TouchTargetSizeCheck,VisualLintBounds" /> 
            </RadioGroup> 
        </LinearLayout> 
        <Button 
            android:id="@+id/btnsub" 
            android:layout_width="wrap_content" 
            android:layout_height="wrap_content" 
            android:layout_gravity="center" 
            android:layout_marginTop="5dp" 
            android:layout_marginBottom="30dp" 
            android:backgroundTint="#e65100" 
            android:padding="20dp" 
            android:text="@string/submit" 
android:textColor="#fff" 
android:textSize="20sp" /> 
</LinearLayout> 
</androidx.constraintlayout.widget.ConstraintLayout> 

c] strings.xml: 
<resources> 
<string name="app_name">Registrationpage</string> 
<string name="registration">Registration</string> 
<string name="name">Name</string> 
<string name="email">Email</string> 
<string name="password">Password</string> 
<string name="roll_no">Roll_no</string> 
<string name="age">Age</string> 
<string name="male">Male</string> 
<string name="female">Female</string> 
<string name="submit">Submit</string> 
</resources>
---------------------------------------------------------------------

4.Create sample application with login module (check 
username and password) & on successful login, change 
TextView to “Login Successful” and on failed login, alert 
user using Toast “Login fail”.  
 
A] Code:  
a] MainActivity.java: 
 
package com.example.loginpage; 
 
import android.os.Bundle; 
import android.view.View; 
import android.widget.Button; 
import android.widget.EditText; 
import android.widget.TextView; 
import android.widget.Toast; 
import androidx.annotation.Nullable; 
import androidx.appcompat.app.AppCompatActivity; 
public class MainActivity extends AppCompatActivity implements View.OnClickListener { 
    TextView txtheadline; 
    EditText edteemail1, edtpw1; 
    Button btnlog; 
    @Override 
    protected void onCreate(@Nullable Bundle savedInstanceState) { 
        super.onCreate(savedInstanceState); 
        setContentView(R.layout.activity_main); 
        // Initialize UI components 
        txtheadline = findViewById(R.id.txthead); 
        edteemail1 = findViewById(R.id.edt_email1); 
        edtpw1 = findViewById(R.id.edt_passwd1); 
        btnlog = findViewById(R.id.btnLog); 
        // Set click listener 
        btnlog.setOnClickListener(this); 
    } 
    @Override 
    public void onClick(View v) { 
// Check login credentials 
        if ((edteemail1.getText().toString().equals("user@gmail.com")) && 
                (edtpw1.getText().toString().equals("1234"))) { 
            Toast.makeText(this, "Login Successful", 
                    Toast.LENGTH_SHORT).show(); 
        } else { 
            Toast.makeText(this, "Login Failed", Toast.LENGTH_SHORT).show(); 
        } 
    } 
} 
b] activity_main.xml: 
<?xml version="1.0" encoding="utf-8"?> 
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android" 
    xmlns:app="http://schemas.android.com/apk/res-auto" 
    xmlns:tools="http://schemas.android.com/tools" 
    android:id="@+id/main" 
    android:layout_width="match_parent" 
    android:layout_height="match_parent" 
    android:background="#FA80CAD5"> 
    <TextView 
        android:id="@+id/txthead" 
        android:layout_width="match_parent" 
        android:layout_height="wrap_content" 
        android:layout_marginLeft="20dp" 
        android:layout_marginTop="40dp" 
        android:layout_marginRight="20dp" 
        android:text="@string/login_form" 
        android:textAlignment="center" 
        android:textColor="#616161" 
        android:textStyle="bold"/> 
    <EditText 
        android:id="@+id/edt_email1" 
        android:layout_width="match_parent" 
        android:layout_height="wrap_content" 
        android:layout_below="@+id/txthead" 
        android:layout_marginLeft="20dp" 
        android:layout_marginTop="20dp" 
        android:layout_marginRight="20dp" 
        android:autofillHints="true" 
        android:text="@string/enter_email" 
        tools:ignore="LabelFor,TextFields,TouchTargetSizeCheck,VisualLintTextFieldSize"/> 
    <EditText 
        android:id="@+id/edt_passwd1" 
        android:layout_width="match_parent" 
        android:layout_height="wrap_content" 
        android:layout_below="@+id/edt_email1" 
        android:layout_marginLeft="20dp" 
        android:layout_marginTop="22dp" 
        android:minHeight="48dp" 
        android:text="@string/enter_password" 
        android:textColorHint="#37474F" 
        
tools:ignore="Autofill,LabelFor,RtlHardcoded,SpeakableTextPresentCheck,TextFields,VisualL
 intTextFieldSize"/> 
    <Button 
        android:id="@+id/btnLog" 
        android:layout_width="match_parent" 
        android:layout_height="wrap_content" 
        android:layout_below="@+id/edt_passwd1" 
        android:layout_marginLeft="60dp" 
        android:layout_marginTop="40dp" 
        android:layout_marginRight="60dp" 
        android:background="#0B8B9B" 
        android:text="Login" 
        android:textColor="#fff" 
        android:textSize="25sp" 
        tools:ignore="HardcodedText,VisualLintButtonSize"/> 
</RelativeLayout> 
 
c] strings.xml: 
<resources> 
    <string name="app_name">Loginpage</string> 
    <string name="login_form">Login Form</string> 
    <string name="enter_email">Enter your email</string> 
    <string name="enter_password">Enter your password</string> 
</resources>
---------------------------------------------------------------------------------

5.Create an application for demonstration of ScrollView in 
Android. 
 
 A] Code: 
  
a] MainActivity.java: 
 
package com.example.scrollview; 
 
import android.os.Bundle; 
import androidx.appcompat.app.AppCompatActivity; 
public class MainActivity extends AppCompatActivity { 
    @Override 
    protected void onCreate(Bundle savedInstanceState) { 
        super.onCreate(savedInstanceState); 
        setContentView(R.layout.activity_main); 
    } 
} 
 
b] activity_main.xml: 
 
<?xml version="1.0" encoding="utf-8"?> 
<androidx.constraintlayout.widget.ConstraintLayout 
xmlns:android="http://schemas.android.com/apk/res/android" 
    xmlns:app="http://schemas.android.com/apk/res-auto" 
    xmlns:tools="http://schemas.android.com/tools" 
    android:id="@+id/main" 
    android:layout_width="match_parent" 
    android:layout_height="match_parent" 
    tools:context=".MainActivity"> 
    <ScrollView 
        android:layout_width="wrap_content" 
        android:layout_height="wrap_content" 
        tools:ignore="MissingConstraints"> 
        <LinearLayout 
            android:layout_width="match_parent" 
            android:layout_height="wrap_content" 
            android:orientation="vertical"> 
            <ImageView 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:layout_marginTop="8dp" 
                android:background="#9C27B0" 
                tools:ignore="ContentDescription,ImageContrastCheck"/> 
            <Button 
                android:layout_width="417dp" 
                android:layout_height="121dp" 
                android:background="#ff5722" 
                android:text="@string/hello_world_1" 
                android:textColor="#212121" 
                tools:ignore="HardcodedText,SpeakableTextPresentCheck,TextContrastChec 
k,VisualLintButtonSize" /> 
            <TextView 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:background="#00BCD4" /> 
            <Button 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:background="@color/black" 
                tools:ignore="SpeakableTextPresentCheck,VisualLintButtonSize" /> 
            <Button 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:background="#673AB7" 
                android:text="@string/hello_world_2" 
                android:textColor="#C5CAE9" 
                tools:ignore="VisualLintButtonSize" /> 
            <ImageView 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:background="#9C27B0" 
                tools:ignore="ContentDescription,ImageContrastCheck" /> 
            <TextView 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:background="#E91E63" /> 
            <Button 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:background="#F44336" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:background="#03A9F4" 
                android:text="@string/hello_world_3" 
                tools:ignore="VisualLintButtonSize" /> 
            <ImageView 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:background="#FF5722" 
                tools:ignore="ContentDescription" /> 
            <TextView 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:background="#FF9800" /> 
            <Button 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:background="#FFEB3B" 
                android:text="@string/hello_world_4" 
                tools:ignore="HardcodedText,VisualLintButtonSize" /> 
            <ImageView 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:background="#FF5722" 
                tools:ignore="ContentDescription" /> 
            <TextView 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:background="#FFA000" /> 
            <Button 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:background="#981874" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:background="#6A7C6B" 
                android:text="@string/hello_world_5" 
                tools:ignore="VisualLintButtonSize" /> 
            <ImageView 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:background="#3F51B5" 
                tools:ignore="ContentDescription" /> 
            <TextView 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:background="#FF0000" /> 
            <Button 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
                android:background="#819012" 
                android:text="@string/hello_world_6" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="match_parent" 
                android:layout_height="200dp" 
android:background="#00FF1A" 
tools:ignore="VisualLintButtonSize"/> 
</LinearLayout> 
</ScrollView> 
</androidx.constraintlayout.widget.ConstraintLayout> 
c] strings.xml: 
<resources> 
<string name="app_name">Scrollview</string> 
<string name="hello_world_1">Hello World 1</string> 
<string name="hello_world_2">Hello World 2</string> 
<string name="hello_world_3">Hello World 3</string> 
<string name="hello_world_4">Hello World 4</string> 
<string name="hello_world_5">Hello World 5</string> 
<string name="hello_world_6">Hello World 6</string>
----------------------------------------------------------------------------------------

6.Create login application where you will have to validate 
username and password till the & username and password 
is not validated, login button should remain disabled. 
A] Code:  
a] MainActivity.java: 
 
package com.example.disabledlogin; 
 
import android.os.Bundle; 
import android.text.Editable; 
import android.text.TextWatcher; 
import android.widget.Button; 
import android.widget.EditText; 
import androidx.appcompat.app.AppCompatActivity; 
public class MainActivity extends AppCompatActivity { 
    private EditText edittextUN; 
    private EditText edittextPass; 
    private Button btnLog; 
    @Override 
    protected void onCreate(Bundle savedInstanceState) { 
        super.onCreate(savedInstanceState); 
        setContentView(R.layout.activity_main); 
        edittextUN = findViewById(R.id.edittxt_Username); 
        edittextPass = findViewById(R.id.edittxt_Password); 
        btnLog = findViewById(R.id.button_Login); 
        edittextUN.addTextChangedListener(loginTextWatcher); 
        edittextPass.addTextChangedListener(loginTextWatcher); 
    } 
    private final TextWatcher loginTextWatcher = new TextWatcher() { 
        @Override 
        public void beforeTextChanged(CharSequence s, int start, int count, int after) { 
        } 
        @Override 
        public void onTextChanged(CharSequence s, int start, int before, int count) { 
            String usernameInput = edittextUN.getText().toString(); 
            String passwordInput = edittextPass.getText().toString(); 
            btnLog.setEnabled(!usernameInput.isEmpty() && !passwordInput.isEmpty()); 
        } 
        @Override 
        public void afterTextChanged(Editable s) { 
        } 
    }; 
} 
b] activity_main.xml: 
<?xml version="1.0" encoding="utf-8"?> 
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android" 
    xmlns:app="http://schemas.android.com/apk/res-auto" 
    xmlns:tools="http://schemas.android.com/tools" 
    android:id="@+id/main" 
    android:layout_width="match_parent" 
    android:layout_height="match_parent" 
    android:layout_margin="20dp" 
    android:layout_gravity="center_horizontal" 
    android:orientation="vertical" 
    android:padding="15dp" 
    tools:context=".MainActivity"> 
    <EditText 
        android:id="@+id/edittxt_Username" 
        android:layout_width="match_parent" 
        android:layout_height="wrap_content" 
        android:layout_marginTop="70dp" 
        android:autofillHints="" 
        android:hint="@string/username" 
        android:inputType="text" 
        android:textColorHint="#78909C" 
        android:textSize="20sp" 
        tools:ignore="VisualLineTextFieldSize,VisualLintTextFieldSize" /> 
    <EditText 
        android:id="@+id/edittxt_Password" 
        android:layout_width="match_parent" 
        android:layout_height="wrap_content" 
        android:hint="@string/password" 
        android:importantForAutofill="no" 
        android:inputType="textPassword" 
        android:textColorHint="#78909C" 
        android:textSize="20sp" 
        tools:ignore="VisualLintTextFieldSize" /> 
 
    <Button 
        android:id="@+id/button_Login" 
        android:layout_width="wrap_content" 
        android:layout_height="wrap_content" 
        android:layout_gravity="center" 
        android:enabled="true" 
        android:text="@string/login" 
        android:textSize="30sp" /> 
</LinearLayout> 
 
c] strings.xml: 
<resources> 
    <string name="app_name">Disabled Login</string> 
 <string name="username">Username</string> 
    <string name="password">Password</string> 
    <string name="login">Login</string> 
</resources>
-----------------------------------------------------------------------------------

7.Create an application for calculator. 
 A] Code:  
a] MainActivity.java: 
package com.example.calculator_pr7; 
 
import android.annotation.SuppressLint; 
import android.os.Bundle; 
import android.widget.Button; 
import android.widget.EditText; 
import android.widget.TextView; 
import android.widget.Toast; 
import androidx.appcompat.app.AppCompatActivity; 
import java.text.DecimalFormat; 
public class MainActivity extends AppCompatActivity { 
    private EditText num1EditText, num2EditText; 
    private TextView resultTextView; 
    @Override 
    protected void onCreate(Bundle savedInstanceState) { 
        super.onCreate(savedInstanceState); 
        setContentView(R.layout.activity_main); 
        num1EditText = findViewById(R.id.num1EditText); 
        num2EditText = findViewById(R.id.num2EditText); 
        resultTextView = findViewById(R.id.resultTextView); 
        Button addButton = findViewById(R.id.addButton); 
        addButton.setOnClickListener(v -> performCalculation('+')); 
        Button subtractButton = findViewById(R.id.subtractButton); 
        subtractButton.setOnClickListener(v -> performCalculation('-')); 
        Button multiplyButton = findViewById(R.id.multiplyButton); 
        multiplyButton.setOnClickListener(v -> performCalculation('*')); 
        Button divideButton = findViewById(R.id.divideButton); 
        divideButton.setOnClickListener(v -> performCalculation('/')); 
        Button sqrtButton = findViewById(R.id.sqrtButton); 
        sqrtButton.setOnClickListener(v -> calculateSquareRoot()); 
    } 
    @SuppressLint("SetTextI18n") 
    private void performCalculation(char operator) { 
        String num1Str = num1EditText.getText().toString(); 
        String num2Str = num2EditText.getText().toString(); 
        if (num1Str.isEmpty() || num2Str.isEmpty()) { 
            Toast.makeText(this, "Please enter both numbers", Toast.LENGTH_SHORT).show(); 
            return; 
        } 
        double num1 = Double.parseDouble(num1Str); 
        double num2 = Double.parseDouble(num2Str); 
        double result = 0; 
        switch (operator) { 
            case '+': 
                result = num1 + num2; 
                break; 
            case '-': 
                result = num1 - num2; 
                break; 
            case '*': 
                result = num1 * num2; 
                break; 
            case '/': 
                if (num2 != 0) { 
                    result = num1 / num2; 
                } else { 
                    Toast.makeText(this, "Cannot divide by zero", Toast.LENGTH_SHORT).show(); 
                    return; 
                } 
                break; 
        } 
        DecimalFormat df = new DecimalFormat("#.##"); 
        resultTextView.setText("Result: " + df.format(result)); 
    } 
    @SuppressLint("SetTextI18n") 
    private void calculateSquareRoot() { 
        String num1Str = num1EditText.getText().toString(); 
        if (num1Str.isEmpty()) { 
            Toast.makeText(this, "Please enter a number", Toast.LENGTH_SHORT).show(); 
            return; 
        } 
        double num = Double.parseDouble(num1Str); 
        double sqrtResult = Math.sqrt(num); 
        DecimalFormat df = new DecimalFormat("#.##"); 
        resultTextView.setText("Square Root: " + df.format(sqrtResult)); 
    } 
} 
 
b] activity_main.xml: 
 
<?xml version="1.0" encoding="utf-8"?> 
<androidx.constraintlayout.widget.ConstraintLayout 
xmlns:android="http://schemas.android.com/apk/res/android" 
    xmlns:app="http://schemas.android.com/apk/res-auto" 
    xmlns:tools="http://schemas.android.com/tools" 
    android:id="@+id/main" 
    android:layout_width="match_parent" 
    android:layout_height="match_parent" 
    android:padding="16dp" 
    tools:context=".MainActivity"> 
    <EditText 
        android:id="@+id/num1EditText" 
        android:layout_width="0dp" 
        android:layout_height="48dp" 
        android:layout_marginTop="44dp" 
        android:hint="Enter number 1" 
        android:inputType="numberDecimal" 
        app:layout_constraintEnd_toEndOf="parent" 
        app:layout_constraintHorizontal_bias="1.0" 
        app:layout_constraintStart_toStartOf="parent" 
        app:layout_constraintTop_toTopOf="parent" 
        tools:ignore="Autofill,HardcodedText,TextContrastCheck,VisualLintTextFieldSize" /> 
    <EditText 
        android:id="@+id/num2EditText" 
        android:layout_width="0dp" 
        android:layout_height="48dp" 
        android:layout_marginTop="32dp" 
        android:hint="Enter number 2" 
        android:inputType="numberDecimal" 
        app:layout_constraintEnd_toEndOf="parent" 
        app:layout_constraintHorizontal_bias="1.0" 
        app:layout_constraintStart_toStartOf="parent" 
        app:layout_constraintTop_toBottomOf="@+id/num1EditText" 
        tools:ignore="Autofill,HardcodedText,TextContrastCheck,VisualLintTextFieldSize" /> 
    <Button 
        android:id="@+id/addButton" 
        android:layout_width="wrap_content" 
        android:layout_height="wrap_content" 
        android:layout_marginTop="20dp" 
        android:background="#5C07F0" 
        android:text="+" 
        android:textColor="@color/white" 
        android:textSize="16sp" 
        app:layout_constraintStart_toStartOf="parent" 
        app:layout_constraintTop_toBottomOf="@+id/num2EditText" 
        tools:ignore="HardcodedText" /> 
    <Button 
        android:id="@+id/subtractButton" 
        android:layout_width="wrap_content" 
        android:layout_height="wrap_content" 
        android:layout_marginTop="20dp" 
        android:background="#5C07F0" 
        android:text="-" 
        android:textColor="@color/white" 
        android:textSize="16sp" 
        app:layout_constraintEnd_toStartOf="@+id/multiplyButton" 
        app:layout_constraintHorizontal_bias="0.582" 
        app:layout_constraintStart_toEndOf="@+id/addButton" 
        app:layout_constraintTop_toBottomOf="@+id/num2EditText" 
        tools:ignore="HardcodedText" /> 
    <Button 
        android:id="@+id/multiplyButton" 
        android:layout_width="wrap_content" 
        android:layout_height="wrap_content" 
        android:layout_marginTop="20dp" 
        android:background="#5C07F0" 
        android:text="x" 
        android:textColor="@color/white" 
        android:textSize="16sp" 
        app:layout_constraintEnd_toEndOf="parent" 
        app:layout_constraintTop_toBottomOf="@+id/num2EditText" 
        tools:ignore="HardcodedText" /> 
    <Button 
        android:id="@+id/divideButton" 
        android:layout_width="wrap_content" 
        android:layout_height="wrap_content" 
        android:layout_marginTop="20dp" 
        android:background="#5C07F0" 
        android:text="/" 
        android:textColor="@color/white" 
        android:textSize="16sp" 
        app:layout_constraintStart_toStartOf="parent" 
        app:layout_constraintTop_toBottomOf="@+id/addButton" 
        tools:ignore="HardcodedText" /> 
    <Button 
        android:id="@+id/sqrtButton" 
        android:layout_width="wrap_content" 
        android:layout_height="wrap_content" 
        android:layout_marginTop="20dp" 
        android:layout_marginEnd="140dp" 
        android:background="#5C07F0" 
        android:text="Sqrt" 
        android:textColor="@color/white" 
        android:textSize="16sp" 
        app:layout_constraintEnd_toEndOf="parent" 
        app:layout_constraintTop_toBottomOf="@+id/subtractButton" 
        tools:ignore="HardcodedText" /> 
    <TextView 
        android:id="@+id/resultTextView" 
        android:layout_width="84dp" 
        android:layout_height="41dp" 
        android:layout_marginStart="4dp" 
        android:layout_marginTop="40dp" 
        android:text="Result: " 
android:textSize="18sp" 
app:layout_constraintStart_toStartOf="parent" 
app:layout_constraintTop_toBottomOf="@+id/divideButton" 
tools:ignore="HardcodedText" /> 
</androidx.constraintlayout.widget.ConstraintLayout>
------------------------------------------------------------------------------------------

8.Demonstrate use of ScrollView. 
1. Vertical ScrollView:  
 1.A] Code:  
a] MainActivity.java: 
package com.example.verticalscrollview; 
 
import android.os.Bundle; 
import androidx.appcompat.app.AppCompatActivity; 
public class MainActivity extends AppCompatActivity { 
    @Override 
    protected void onCreate(Bundle savedInstanceState) { 
        super.onCreate(savedInstanceState); 
        setContentView(R.layout.activity_main); 
    } 
} 
 
b] activity_main.xml: 
 
<?xml version="1.0" encoding="utf-8"?> 
<!--suppress ALL --> 
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android" 
    xmlns:app="http://schemas.android.com/apk/res-auto" 
    xmlns:tools="http://schemas.android.com/tools" 
    android:id="@+id/main" 
    android:layout_width="match_parent" 
    android:layout_height="match_parent" 
    android:orientation="vertical" 
    tools:context=".MainActivity"> 
    <ScrollView 
        android:id="@+id/scrollView" 
        android:layout_width="fill_parent" 
        android:layout_height="wrap_content" 
        android:layout_marginTop="20dp" 
        tools:ignore="UselessParent"> 
        <LinearLayout 
            android:layout_width="fill_parent" 
            android:layout_height="wrap_content" 
            android:orientation="vertical"> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:background="@color/design_default_color_primary" 
                android:text="vertical_scroll_view" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_2" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_3" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_4" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_5" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_6" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_7" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_8" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_9" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_10" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_11" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_12" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="Button 13" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="HardcodedText,VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_14" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_15" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_16" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_17" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_18" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_19" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
            <Button 
                android:layout_width="fill_parent" 
                android:layout_height="wrap_content" 
                android:layout_marginTop="10sp" 
                android:background="@color/design_default_color_primary" 
                android:text="@string/button_20" 
                android:textAlignment="center" 
                android:textColor="#ffffff" 
                tools:ignore="VisualLintButtonSize" /> 
        </LinearLayout> 
    </ScrollView> 
</LinearLayout> 
 
c] strings.xml: 
<resources> 
    <string name="app_name">Vertical Scroll View</string> 
    <string name="Vertical_scroll_view">Vertical Scroll View</string> 
    <string name="button_2">Button 2</string> 
    <string name="button_3">Button 3</string> 
    <string name="button_4">Button 4</string> 
    <string name="button_5">Button 5</string> 
    <string name="button_6">Button 6</string> 
    <string name="button_7">Button 7</string> 
    <string name="button_8">Button 8</string> 
<string name="button_9">Button 9</string> 
<string name="button_10">Button 10</string> 
<string name="button_11">Button 11</string> 
<string name="button_12">Button 12</string> 
<string name="button_13">Button 13</string> 
<string name="button_14">Button 14</string> 
<string name="button_15">Button 15</string> 
<string name="button_16">Button 16</string> 
<string name="button_17">Button 17</string> 
<string name="button_18">Button 18</string> 
<string name="button_19">Button 19</string> 
<string name="button_20">Button 20</string> 
</resources>
-------------------------------------------------------------------------------
2. Horizontal ScrollView: 
2.A] Code:  
a] MainActivity.java: 
 
package com.example.horizontalscrollview; 
 
import android.os.Bundle; 
import androidx.appcompat.app.AppCompatActivity; 
public class MainActivity extends AppCompatActivity { 
    @Override 
    protected void onCreate(Bundle savedInstanceState) { 
        super.onCreate(savedInstanceState); 
        setContentView(R.layout.activity_main); 
    } 
} 
 
b] activity_main.xml: 
 
<?xml version="1.0" encoding="utf-8"?> 
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android" 
    xmlns:app="http://schemas.android.com/apk/res-auto" 
    xmlns:tools="http://schemas.android.com/tools" 
    android:id="@+id/main" 
    android:layout_width="match_parent" 
    android:layout_height="match_parent" 
    android:orientation="vertical" 
    android:padding="15dp" 
    tools:context=".MainActivity"> 
 
    <HorizontalScrollView 
        android:layout_width="match_parent" 
        android:layout_height="wrap_content" 
        tools:ignore="SpeakableTextPresentCheck,UselessParent"> 
        <LinearLayout 
            android:layout_width="wrap_content" 
            android:layout_height="match_parent" 
            android:orientation="horizontal" 
            tools:ignore="VisualLintBounds"> 
 
            <ImageView 
                android:layout_width="150dp" 
                android:layout_height="150dp" 
                android:layout_marginTop="120dp" 
                android:layout_marginEnd="5dp" 
                android:scaleType="centerCrop" 
                android:src="@drawable/image1" 
                tools:ignore="ContentDescription,ImageContrastCheck" /> 
            <ImageView 
                android:layout_width="150dp" 
                android:layout_height="150dp" 
                android:layout_marginEnd="5dp" 
                android:layout_marginTop="120dp" 
                android:scaleType="centerCrop" 
                android:src="@drawable/image2" 
                tools:ignore="ContentDescription" /> 
            <ImageView 
                android:layout_width="150dp" 
                android:layout_height="150dp" 
                android:layout_marginTop="120dp" 
                android:layout_marginEnd="5dp" 
                android:scaleType="centerCrop" 
                android:src="@drawable/image3" 
                tools:ignore="ContentDescription" /> 
            <ImageView 
                android:layout_width="150dp" 
                android:layout_height="150dp" 
                android:layout_marginEnd="5dp" 
                android:layout_marginTop="120dp" 
                android:scaleType="centerCrop" 
                android:src="@drawable/image4" 
                tools:ignore="ContentDescription" /> 
            <ImageView 
                android:layout_width="150dp" 
                android:layout_height="150dp" 
                android:layout_marginRight="5dp" 
                android:layout_marginTop="120dp" 
                android:scaleType="centerCrop" 
                android:src="@drawable/image5" 
                tools:ignore="ContentDescription,RtlHardcoded" /> 
        </LinearLayout> 
    </HorizontalScrollView> 
</LinearLayout>
-----------------------------------------------------------------------------------------------

9.Demonstrate use of Intent in Android. 
A] Code:  
a] MainActivity.java: 
package com.example.intent; 
 
import android.os.Bundle; 
import androidx.appcompat.app.AppCompatActivity; 
import android.content.Intent; 
import android.net.Uri; 
import android.view.View; 
import android.widget.Button; 
/** 
 * @noinspection ALL 
 */ 
public class MainActivity extends AppCompatActivity { 
    @Override 
    protected void onCreate(Bundle savedInstanceState) { 
        super.onCreate(savedInstanceState); 
        setContentView(R.layout.activity_main); 
        Button email = findViewById(R.id.openEmail); 
        Button gallery = findViewById(R.id.openGallery); 
        Button dialer = findViewById(R.id.openDialer); 
        email.setOnClickListener(new View.OnClickListener() { 
            @Override 
            public void onClick(View v) { 
                Intent intent = new Intent(Intent.ACTION_SENDTO); 
                intent.setData(Uri.parse("mailto:")); 
                intent.putExtra(Intent.EXTRA_EMAIL, "Dnc@gmail.com"); 
                intent.putExtra(Intent.EXTRA_SUBJECT, "Android App Practice"); 
                startActivity(intent); 
            } 
        }); 
        gallery.setOnClickListener(new View.OnClickListener() { 
            @Override 
            public void onClick(View v) { 
                Intent intent = new Intent(); 
                intent.setAction(android.content.Intent.ACTION_VIEW); 
                intent.setType("image/*"); 
                intent.setFlags(Intent.FLAG_ACTIVITY_NEW_TASK); 
                startActivity(intent); 
            } 
        }); 
        dialer.setOnClickListener(new View.OnClickListener() { 
            @Override 
            public void onClick(View v) { 
                Intent intent = new Intent(Intent.ACTION_DIAL); 
                intent.setData(Uri.parse("tel:2613401000")); 
                startActivity(intent); 
            } 
        }); 
    } 
} 
b] activity_main.xml: 
<?xml version="1.0" encoding="utf-8"?> 
<androidx.constraintlayout.widget.ConstraintLayout 
xmlns:android="http://schemas.android.com/apk/res/android" 
    xmlns:app="http://schemas.android.com/apk/res-auto" 
    xmlns:tools="http://schemas.android.com/tools" 
    android:id="@+id/main" 
    android:layout_width="match_parent" 
    android:layout_height="match_parent" 
    tools:context=".MainActivity"> 
    <Button 
        android:id="@+id/openEmail" 
        android:layout_width="177dp" 
        android:layout_height="48dp" 
        android:backgroundTint="#2962FF" 
        android:text="@string/open_email_app" 
        app:layout_constraintBottom_toBottomOf="parent" 
        app:layout_constraintEnd_toEndOf="parent" 
        app:layout_constraintHorizontal_bias="0.467" 
        app:layout_constraintStart_toStartOf="parent" 
        app:layout_constraintTop_toTopOf="parent" 
        app:layout_constraintVertical_bias="0.197" /> 
    <Button 
        android:id="@+id/openGallery" 
        android:layout_width="177dp" 
        android:layout_height="48dp" 
        android:backgroundTint="#D50000" 
        android:text="@string/open_gallery_app" 
        app:layout_constraintBottom_toTopOf="@+id/openDialer" 
        app:layout_constraintEnd_toEndOf="parent" 
        app:layout_constraintHorizontal_bias="0.465" 
        app:layout_constraintStart_toStartOf="parent" 
        app:layout_constraintTop_toBottomOf="@+id/openEmail" /> 
    <Button 
        android:id="@+id/openDialer" 
        android:layout_width="176dp" 
        android:layout_height="49dp" 
        android:layout_marginTop="4dp" 
        android:backgroundTint="#64DD17" 
        android:text="@string/open_phone_dialer" 
android:textColor="#5E35B1" 
app:layout_constraintEnd_toEndOf="parent" 
app:layout_constraintHorizontal_bias="0.468" 
app:layout_constraintStart_toStartOf="parent" 
app:layout_constraintTop_toBottomOf="@+id/openGallery" /> 
</androidx.constraintlayout.widget.ConstraintLayout> 
c] strings.xml: 
<resources> 
<string name="app_name">Intent</string> 
<string name="open_email_app">Open Email App</string> 
<string name="open_gallery_app">Open Gallery</string> 
<string name="open_phone_dialer">Open Phone Dialer</string>
------------------------------------------------------------------------

10.Create application to demonstrate menu option. 
1.Options Menu: 
1.A] Code:  
a] MainActivity.java: 
package com.example.menuoptions; 
 
import android.os.Bundle; 
 
import android.view.Menu; 
import android.view.MenuItem; 
import android.widget.Toast; 
import androidx.annotation.NonNull; 
import androidx.appcompat.app.AppCompatActivity; 
 
public class MainActivity extends AppCompatActivity { 
 
    @Override 
    protected void onCreate(Bundle savedInstanceState) { 
        super.onCreate(savedInstanceState); 
        setContentView(R.layout.activity_main); 
    } 
    @Override 
    public boolean onCreateOptionsMenu(Menu menu) { 
        // return super.onCreateOptionsMenu(menu); 
        getMenuInflater().inflate(R.menu.menu, menu); 
        return true; 
    } 
    @Override 
    public boolean onOptionsItemSelected(@NonNull MenuItem item) { 
        int id = item.getItemId(); 
        if (id == R.id.item1) { 
            Toast.makeText(this, "Item 1 selected", Toast.LENGTH_SHORT).show(); 
        } else if (id == R.id.item2) { 
            Toast.makeText(this, "Item 2 selected", Toast.LENGTH_SHORT).show(); 
        } else if (id == R.id.item3) { 
            Toast.makeText(this, "Item 3 selected", Toast.LENGTH_SHORT).show(); 
        } else { 
            return super.onOptionsItemSelected(item); 
        } 
        return true; 
    } 
} 
b] activity_main.xml: 
<?xml version="1.0" encoding="utf-8"?> 
<androidx.constraintlayout.widget.ConstraintLayout 
xmlns:android="http://schemas.android.com/apk/res/android" 
    xmlns:app="http://schemas.android.com/apk/res-auto" 
    xmlns:tools="http://schemas.android.com/tools" 
    android:id="@+id/main" 
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
c]menu.xml: 
 
<?xml version="1.0" encoding="utf-8"?> 
<menu xmlns:android="http://schemas.android.com/apk/res/android"> 
    <item 
        android:title="@string/item1" 
        android:id="@+id/item1"/> 
    <item 
        android:title="@string/item2" 
        android:id="@+id/item2"/> 
    <item 
        android:title="@string/item3" 
        android:id="@+id/item3"/> 
</menu> 
 
c] strings.xml: 
<resources> 
    <string name="app_name">MenuOptions</string> 
    <string name="item1">Item 1</string> 
    <string name="item3">Item 2</string> 
    <string name="item2">Item 3</string> 
</resources> 
 
d] themes.xml: 
<resources xmlns:tools="http://schemas.android.com/tools"> 
    <!-- Base application theme. --> 
    <style name="Base.Theme.MenuOptions" 
parent="Theme.AppCompat.DayNight.DarkActionBar"> 
        <!-- Customize your light theme here. --> 
        <!-- <item name="colorPrimary">@color/my_light_primary</item> --> 
</style> 
<style name="Theme.MenuOptions" parent="Base.Theme.MenuOptions" /> 
</resources> 
e] themes.xml: 
<resources xmlns:tools="http://schemas.android.com/tools"> 
<!-- Base application theme. --> 
<style name="Base.Theme.MenuOptions" 
parent="Theme.AppCompat.DayNight.DarkActionBar"> 
<!-- Customize your dark theme here. --> 
<!-- <item name="colorPrimary">@color/my_dark_primary</item> --> 
</style> 
</resources>
------------------------------------------------------------------------------------

2.Context Menu: 
2.A] Code:  
a] MainActivity.java: 
package com.example.contextmenu; 
 
import android.os.Bundle; 
import android.view.ContextMenu; 
import android.view.MenuInflater; 
import android.view.MenuItem; 
import android.view.View; 
import android.widget.ArrayAdapter; 
import android.widget.ListView; 
import android.widget.Toast; 
import androidx.appcompat.app.AppCompatActivity; 
/** @noinspection RedundantCast, CStyleArrayDeclaration */ 
public class MainActivity extends AppCompatActivity { 
    ListView listView; 
    String contacts[]={"Abhishek","Ashish","Piyush","Shraddha","Chaitali"}; 
    @Override 
    protected void onCreate(Bundle savedInstanceState) { 
        super.onCreate(savedInstanceState); 
        setContentView(R.layout.activity_main); 
        listView=(ListView)findViewById(R.id.listView); 
        ArrayAdapter<String> adapter= new ArrayAdapter<>(this, 
android.R.layout.simple_list_item_1, contacts); 
        listView.setAdapter(adapter); 
        registerForContextMenu(listView); 
    } 
    @Override 
    public void onCreateContextMenu(ContextMenu menu, View v, 
ContextMenu.ContextMenuInfo menuInfo) { 
        super.onCreateContextMenu(menu, v, menuInfo); 
        MenuInflater inflater = getMenuInflater(); 
        inflater.inflate(R.menu.mainmenu, menu); 
        menu.setHeaderTitle("Select The Action"); 
    } 
    @Override 
    public boolean onContextItemSelected(MenuItem item){ 
        if(item.getItemId()==R.id.call) { 
            Toast.makeText(getApplicationContext(), "calling code", 
Toast.LENGTH_LONG).show(); 
        } 
        else if(item.getItemId()==R.id.sms){ 
            Toast.makeText(getApplicationContext(),"sending sms 
code",Toast.LENGTH_LONG).show(); 
        }else{ 
            return false; 
        } 
        return true; 
    } 
} 
 
b] activity_main.xml: 
<?xml version="1.0" encoding="utf-8"?> 
<androidx.constraintlayout.widget.ConstraintLayout 
xmlns:android="http://schemas.android.com/apk/res/android" 
    xmlns:app="http://schemas.android.com/apk/res-auto" 
    xmlns:tools="http://schemas.android.com/tools" 
    android:id="@+id/main" 
    android:layout_width="match_parent" 
    android:layout_height="match_parent" 
    tools:context=".MainActivity" 
    tools:ignore="VisualLintBounds"> 
    <ListView 
        android:id="@+id/listView" 
        android:layout_width="334dp" 
        android:layout_height="441dp" 
        android:layout_marginStart="8dp" 
        android:layout_marginTop="132dp" 
        android:layout_marginEnd="8dp" 
        app:layout_constraintEnd_toEndOf="parent" 
        app:layout_constraintHorizontal_bias="0.295" 
        app:layout_constraintStart_toStartOf="parent" 
        app:layout_constraintTop_toTopOf="parent" /> 
</androidx.constraintlayout.widget.ConstraintLayout> 
 
c] mainmenu.xml: 
 
<?xml version="1.0" encoding="utf-8"?> 
<menu xmlns:android="http://schemas.android.com/apk/res/android"> 
    <item 
        android:id="@+id/call" 
        android:title="@string/call" /> 
    <item android:id="@+id/sms" 
        android:title="@string/sms" /> 
</menu> 
 
d] strings.xml:  
<resources> 
    <string name="app_name">ContextMenu</string> 
    <string name="call">Call</string> 
<string name="sms">SMS</string> 
</resources> 
-------------------------------------------------------------------------

3.Popup Menu: 
3.A] Code:  
a] MainActivity.java: 
package com.example.popup_menu; 
 
import android.os.Bundle; 
import android.view.MenuItem; 
import android.view.View; 
import android.widget.Button; 
import android.widget.PopupMenu; 
import android.widget.Toast; 
import androidx.appcompat.app.AppCompatActivity; 
/** @noinspection Convert2Lambda*/ 
public class MainActivity extends AppCompatActivity { 
    Button button; 
    @Override 
    protected void onCreate(Bundle savedInstanceState) { 
        super.onCreate(savedInstanceState); 
        setContentView(R.layout.activity_main); 
        button = findViewById(R.id.button); // Casting is not needed 
        button.setOnClickListener(new View.OnClickListener() { 
            @Override 
            public void onClick(View view) { 
                PopupMenu popupMenu = new PopupMenu(MainActivity.this, button); 
                popupMenu.getMenuInflater().inflate(R.menu.popup_menu, 
popupMenu.getMenu()); 
                popupMenu.setOnMenuItemClickListener(new 
PopupMenu.OnMenuItemClickListener() { 
                    @Override 
                    public boolean onMenuItemClick(MenuItem menuItem) { 
                        Toast.makeText(MainActivity.this, "You Clicked " + menuItem.getTitle(), 
Toast.LENGTH_SHORT).show(); 
                        return true; 
                    } 
                }); 
                popupMenu.show(); 
            } 
        }); 
    } 
} 
b] activity_main.xml: 
<?xml version="1.0" encoding="utf-8"?> 
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android" 
    xmlns:app="http://schemas.android.com/apk/res-auto" 
    xmlns:tools="http://schemas.android.com/tools" 
    android:id="@+id/main" 
    android:layout_width="match_parent" 
    android:layout_height="match_parent" 
    android:gravity="center" 
    android:orientation="vertical"> 
    <Button 
        android:id="@+id/button" 
        android:layout_width="wrap_content" 
        android:layout_height="wrap_content" 
        android:text="@string/show_popup_menu" /> 
</LinearLayout> 
c] popup_menu.xml: 
 
<?xml version="1.0" encoding="utf-8"?> 
<menu xmlns:android="http://schemas.android.com/apk/res/android"> 
    <item android:id="@+id/one" android:title="@string/one" /> 
    <item android:id="@+id/two" android:title="@string/two" /> 
    <item android:id="@+id/three" android:title="@string/three" /> 
</menu> 
 
d] strings.xml:  
<resources> 
    <string name="app_name">POPUP_MENU</string> 
    <string name="show_popup_menu">Show Popup Menu</string> 
    <string name="one">One</string> 
    <string name="two">Two</string> 
    <string name="three">Three</string> 
</resources>
------------------------------------------------------------------------------------

11. Create application to demonstrate progress bar. 
 
 A] Code:  
a] MainActivity.java: 
package com.example.progress_bar; 
 
import android.os.Bundle; 
import android.app.ProgressDialog; 
import android.os.Handler; 
import android.view.View; 
import android.widget.Button; 
import androidx.appcompat.app.AppCompatActivity; 
/** @noinspection ALL*/ 
public class MainActivity extends AppCompatActivity { 
    Button btnStartProgress; 
    ProgressDialog progressBar; 
    private int progressBarStatus = 0; 
    private Handler progressBarHandler = new Handler(); 
    private long fileSize = 0; 
    @Override 
    protected void onCreate(Bundle savedInstanceState) { 
        super.onCreate(savedInstanceState); 
        setContentView(R.layout.activity_main); 
       addListenerOnButtonClick(); 
    } 
    public void addListenerOnButtonClick() { 
        btnStartProgress = findViewById(R.id.button1); 
        btnStartProgress.setOnClickListener(new View.OnClickListener() { 
            @Override 
            public void onClick(View v) { 
                progressBar = new ProgressDialog(MainActivity.this); 
                progressBar.setCancelable(true); 
                progressBar.setMessage("File downloading....."); 
                progressBar.setProgressStyle(ProgressDialog.STYLE_HORIZONTAL); 
                progressBar.setProgress(0); 
                progressBar.setMax(100); 
                progressBar.show(); 
                progressBarStatus = 0; 
                fileSize = 0; 
 
                new Thread(new Runnable() { 
                    @Override 
                    public void run() { 
                        while (progressBarStatus < 100) { 
                            progressBarStatus = doOperation(); 
                            try { 
                                Thread.sleep(1000); 
                            } catch (InterruptedException e) { 
                                e.printStackTrace(); 
                            } 
                            progressBarHandler.post(new Runnable() { 
                                @Override 
                                public void run() { 
                                    progressBar.setProgress(progressBarStatus); 
                                } 
                            }); 
                        } 
                        if (progressBarStatus >= 100) { 
                            try { 
                                Thread.sleep(1000); 
                            } catch (InterruptedException e) { 
                                e.printStackTrace(); 
                            } 
                            progressBar.dismiss(); 
                        } 
                    } 
                }).start(); 
            } 
        }); 
    } 
 
    public int doOperation() { 
        if (fileSize < 10000) { 
            fileSize += 1000;  // Increment by 1000 for a smoother progress 
            return (int) ((fileSize / 10000.0) * 100); // Return percentage 
        } 
        return 100;  // Once fileSize reaches 10000, return 100% 
    } 
} 
 
b] activity_main.xml: 
<?xml version="1.0" encoding="utf-8"?> 
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android" 
    xmlns:app="http://schemas.android.com/apk/res-auto" 
    xmlns:tools="http://schemas.android.com/tools" 
    android:id="@+id/main" 
    android:layout_width="match_parent" 
    android:layout_height="match_parent" 
    tools:context=".MainActivity"> 
    <Button 
        android:id="@+id/button1" 
        android:layout_width="wrap_content" 
        android:layout_height="wrap_content" 
android:layout_alignParentTop="true" 
android:layout_centerHorizontal="true" 
android:layout_marginTop="116dp" 
android:text="@string/download_file"/> 
</RelativeLayout> 
c] strings.xml: 
<resources> 
<string name="app_name">Progress_Bar</string> 
<string name="download_file">Download File</string> 
</resources>
----------------------------------------------------------------------


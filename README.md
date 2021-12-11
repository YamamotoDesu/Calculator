# **[Calculator](https://www.youtube.com/watch?v=uRyvNKRkwbs&t=24046s)** 
Kotlin Android Tutorial by Denis Panjuta

<img width="365" alt="Android_Emulator_-_Nexus_6_API_30_5554" src="https://user-images.githubusercontent.com/47273077/145665964-0aca7502-fad5-4dd5-bdbb-b990c7db4b44.png">


```xml

<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity"
    android:orientation="vertical"
    >

    <TextView
        android:id="@+id/tvInput"
        android:layout_width="match_parent"
        android:layout_height="250dp"
        android:padding="10dp"
        android:textSize="48sp"
        android:text=""
        android:maxLength="12"
        android:textColor="@color/black"
        android:gravity="right|bottom|center_vertical"/>

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal"
        android:layout_weight="1"
        >

        <Button
            android:id="@+id/button7"
            android:layout_width="0dp"
            android:layout_height="match_parent"
            android:layout_margin="2dp"
            android:layout_weight="1"
            android:textSize="45sp"
            android:gravity="center"
            android:includeFontPadding="false"
            android:onClick="onDigit"
            android:text="@string/_7" />

        <Button
            android:id="@+id/button8"
            android:layout_width="0dp"
            android:layout_margin="2dp"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:textSize="45sp"
            android:gravity="center"
            android:includeFontPadding="false"
            android:onClick="onDigit"
            android:text="@string/_8" />
        <Button
            android:id="@+id/button9"
            android:layout_width="0dp"
            android:layout_margin="2dp"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:textSize="45sp"
            android:gravity="center"
            android:includeFontPadding="false"
            android:onClick="onDigit"
            android:text="@string/_9" />
        <Button
            android:id="@+id/buttonDivide"
            android:layout_width="0dp"
            android:layout_margin="2dp"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:textSize="45sp"
            android:gravity="center"
            android:includeFontPadding="false"
            android:text="@string/Multiply"
            android:onClick="onOperator"
            />
    </LinearLayout>

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal"
        android:layout_weight="1"
        >
        <Button
            android:id="@+id/button4"
            android:layout_width="0dp"
            android:layout_margin="2dp"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:textSize="45sp"
            android:gravity="center"
            android:includeFontPadding="false"
            android:onClick="onDigit"
            android:text="@string/_4"/>
        <Button
            android:id="@+id/button5"
            android:layout_width="0dp"
            android:layout_margin="2dp"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:textSize="45sp"
            android:gravity="center"
            android:includeFontPadding="false"
            android:onClick="onDigit"
            android:text="@string/_5" />

        <Button
            android:id="@+id/button6"
            android:layout_width="0dp"
            android:layout_margin="2dp"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:textSize="45sp"
            android:gravity="center"
            android:includeFontPadding="false"
            android:onClick="onDigit"
            android:text="@string/_6" />

        <Button
            android:id="@+id/buttonMultiply"
            android:layout_width="0dp"
            android:layout_margin="2dp"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:textSize="45sp"
            android:gravity="center"
            android:includeFontPadding="false"
            android:text="@string/Divide"
            android:onClick="onOperator" />
    </LinearLayout>

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal"
        android:layout_weight="1"
        >
        <Button
            android:id="@+id/button1"
            android:layout_width="0dp"
            android:layout_margin="2dp"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:textSize="45sp"
            android:gravity="center"
            android:includeFontPadding="false"
            android:onClick="onDigit"
            android:text="@string/_1"/>
        <Button
            android:id="@+id/button2"
            android:layout_width="0dp"
            android:layout_margin="2dp"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:textSize="45sp"
            android:gravity="center"
            android:includeFontPadding="false"
            android:onClick="onDigit"
            android:text="@string/_2"/>
        <Button
            android:id="@+id/button3"
            android:layout_width="0dp"
            android:layout_margin="2dp"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:textSize="45sp"
            android:gravity="center"
            android:includeFontPadding="false"
            android:onClick="onDigit"
            android:text="@string/_3"/>
        <Button
            android:id="@+id/buttonSubtract"
            android:layout_width="0dp"
            android:layout_margin="2dp"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:textSize="45sp"
            android:gravity="center"
            android:includeFontPadding="false"
            android:text="@string/Minus"
            android:onClick="onOperator"
            />


    </LinearLayout>

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal"
        android:layout_weight="1"
        >
        <Button
            android:id="@+id/buttonDot"
            android:layout_width="0dp"
            android:layout_margin="2dp"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:textSize="45sp"
            android:gravity="center"
            android:includeFontPadding="false"
            android:onClick="onDecimalPoint"
            android:text="@string/Dot"/>
        <Button
            android:id="@+id/button0"
            android:layout_width="0dp"
            android:layout_margin="2dp"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:textSize="45sp"
            android:gravity="center"
            android:includeFontPadding="false"
            android:onClick="onDigit"
            android:text="@string/zero"/>

        <Button
            android:id="@+id/buttonCLR"
            android:layout_width="0dp"
            android:layout_margin="2dp"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:textSize="30sp"
            android:gravity="center"
            android:includeFontPadding="false"
            android:onClick="onCLR"
            android:text="@string/clr"/>
        <Button
            android:id="@+id/buttonAdd"
            android:layout_width="0dp"
            android:layout_margin="2dp"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:textSize="45sp"
            android:gravity="center"
            android:includeFontPadding="false"
            android:text="@string/plus"
            android:onClick="onOperator"
            />

    </LinearLayout>

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal"
        android:layout_weight="1"
        >

        <Button
            android:id="@+id/buttonEqual"
            android:layout_width="0dp"
            android:layout_margin="2dp"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:textSize="45sp"
            android:gravity="center"
            android:includeFontPadding="false"
            android:text="@string/equal"
            android:onClick="onEqual"
            />
    </LinearLayout>
</LinearLayout>

```

# Franssen-Properties
This is going to be the layout of the activities in Franssen Properties app. 

This is the same first screen but with the landscape layout

<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#0099cc"
    android:orientation="vertical"
    tools:context="com.example.edwingariza.franssenproperties.FullscreenActivity">
    <FrameLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:fitsSystemWindows="true">

        <LinearLayout
            android:id="@+id/fullscreen_content_controls"
            style="?metaButtonBarStyle"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_gravity="bottom|center_horizontal"
            android:background="@color/black_overlay"
            android:orientation="horizontal"
            tools:ignore="UselessParent">

        </LinearLayout>
    </FrameLayout>

    <TextView
        android:id="@+id/fullscreen_content"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:gravity="center"
        android:keepScreenOn="true"
        android:text="@string/dummy_content"
        android:textColor="#33b5e5"
        android:textSize="50sp"
        android:textStyle="bold" />
    <ImageButton
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:contentDescription="@string/overflow_menu"
        android:onClick="showPopup"/>

    <Button
        android:text="@string/explore_button"

        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:id="@+id/button2"
        android:layout_above="@+id/imageButton"
        android:layout_alignParentRight="true"
        android:layout_alignParentEnd="true"
        android:layout_marginBottom="92dp" />

    <Button
        android:text="@string/login_button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:id="@+id/button"
        android:layout_below="@+id/imageButton2"
        android:layout_alignParentRight="true"
        android:layout_alignParentEnd="true"
        android:layout_marginTop="73dp" />

    <ImageButton
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:srcCompat="@android:drawable/btn_star_big_on"
        android:id="@+id/imageButton"
        android:layout_alignParentBottom="true"
        android:layout_alignParentLeft="true"
        android:layout_alignParentStart="true" />


</RelativeLayout>

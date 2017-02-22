<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#0099cc"
    tools:context="com.example.edwingariza.franssenproperties.FullscreenActivity">

    <!-- The primary full-screen view. This can be replaced with whatever view
         is needed to present your content, e.g. VideoView, SurfaceView,
         TextureView, etc. -->

    <!-- This FrameLayout insets its children based on system windows using
         android:fitsSystemWindows. -->
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

            <Button
                android:id="@+id/dummy_button"
                style="?metaButtonBarButtonStyle"
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="@string/dummy_button" />

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
        android:text="@string/login_button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:id="@+id/button"
        android:layout_alignBaseline="@+id/button2"
        android:layout_alignBottom="@+id/button2"
        android:layout_toLeftOf="@+id/button2"
        android:layout_toStartOf="@+id/button2"
        android:layout_marginRight="70dp"
        android:layout_marginEnd="70dp" />

    <Button
        android:text="@string/explore_button"

        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:id="@+id/button2"
        android:layout_marginRight="64dp"
        android:layout_marginEnd="64dp"
        android:layout_marginBottom="65dp"
        android:layout_alignParentBottom="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentEnd="true" />

    <ImageButton
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:srcCompat="@android:drawable/btn_star_big_on"
        android:id="@+id/imageButton"
        android:layout_alignTop="@+id/button2"
        android:layout_alignParentRight="true"
        android:layout_alignParentEnd="true"
        android:layout_marginTop="15dp" />

</RelativeLayout>

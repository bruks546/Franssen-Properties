
# Franssen-Properties


This are the menu items for most of the activities 

<menu xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    tools:context="com.example.edwingariza.franssenproperties.ScrollingActivity">
    <item
        android:id="@+id/action_settings"
        android:orderInCategory="500"
        android:title="@string/action_settings"
        app:showAsAction="never" />

    <item
        android:id="@+id/my_account"
        android:orderInCategory="100"
        android:title="@string/my_account"
        app:showAsAction="never" />
    <item
        android:id="@+id/favorites"
        android:orderInCategory="200"
        android:title="@string/favorites"
        app:showAsAction="never" />
    <item
        android:id="@+id/rent_calculator"
        android:orderInCategory="300"
        android:title="@string/rent_calculator"
        app:showAsAction="never"/>
    <item
        android:id="@+id/apply"
        android:orderInCategory="400"
        android:title="@string/apply"
        app:showAsAction="never"/>
    <item
        android:id="@+id/contact_us"
        android:title="@string/conract_us"
        android:orderInCategory="500"
        app:showAsAction="never"/>
    <item
        android:id="@+id/about"
        android:title="@string/about"
        android:orderInCategory="700"
        app:showAsAction="never"/>
    <item
        android:id="@+id/feedback"
        android:orderInCategory="800"
        android:title="@string/feedback" />

</menu>
=======
This is going to be the layout of the activities in Franssen Properties app. 


This are the pics that I would be using.  I will need more but I will get them later. 
https://goo.gl/photos/S2SfrDPyx1JbRWDu9

<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:gravity="center_horizontal"
    android:orientation="vertical"
    android:paddingBottom="@dimen/activity_vertical_margin"
    android:paddingLeft="@dimen/activity_horizontal_margin"
    android:paddingRight="@dimen/activity_horizontal_margin"
    android:paddingTop="@dimen/activity_vertical_margin"
    tools:context="com.example.edwingariza.testscreens.LoginActivity">

    <!-- Login progress -->
    <ProgressBar
        android:id="@+id/login_progress"
        style="?android:attr/progressBarStyleLarge"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginBottom="8dp"
        android:visibility="gone" />

    <ScrollView
        android:id="@+id/login_form"
        android:layout_width="match_parent"
        android:layout_height="match_parent">

        <LinearLayout
            android:id="@+id/email_login_form"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:orientation="vertical">

            <android.support.design.widget.TextInputLayout
                android:layout_width="match_parent"
                android:layout_height="wrap_content">

                <AutoCompleteTextView
                    android:id="@+id/email"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:hint="@string/prompt_email"
                    android:inputType="textEmailAddress"
                    android:maxLines="1"
                    android:singleLine="true" />

            </android.support.design.widget.TextInputLayout>

            <android.support.design.widget.TextInputLayout
                android:layout_width="match_parent"
                android:layout_height="wrap_content">

                <EditText
                    android:id="@+id/password"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:hint="@string/prompt_password"
                    android:imeActionId="@+id/login"
                    android:imeActionLabel="@string/action_sign_in_short"
                    android:imeOptions="actionUnspecified"
                    android:inputType="textPassword"
                    android:maxLines="1"
                    android:singleLine="true" />

            </android.support.design.widget.TextInputLayout>

            <Button
                android:id="@+id/email_sign_in_button"
                style="?android:textAppearanceSmall"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginTop="16dp"
                android:text="@string/action_sign_in"
                android:textStyle="bold" />

        </LinearLayout>
    </ScrollView>
</LinearLayout>
=======
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



![image](https://github.com/user-attachments/assets/a2658daf-19d5-4d1e-95e1-70a837dce8bf)

## Add Dependencies
implementation("nl.joery.animatedbottombar:library:1.1.0")

## Add this in activity_main.xml

<nl.joery.animatedbottombar.AnimatedBottomBar
        android:id="@+id/bottom_bar"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:background="#FFF"
        app:abb_indicatorAppearance="round"
        app:abb_indicatorHeight="4dp"
        app:abb_indicatorMargin="16dp"
        app:abb_selectedIndex="0"
        app:abb_selectedTabType="text"
        app:abb_tabs="@menu/tabs"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent" />


## Create menu dir in res, and in that create tabs.xml
<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:android="http://schemas.android.com/apk/res/android">
    <item
        android:id="@+id/tab_home"
        android:icon="@drawable/home"
        android:title="home" />
    <item
        android:id="@+id/tab_alarm"
        android:icon="@drawable/alarm"
        android:title="alarm" />
    <item
        android:id="@+id/tab_bread"
        android:icon="@drawable/bread"
        android:title="bread" />
    <item
        android:id="@+id/tab_cart"
        android:icon="@drawable/cart"
        android:title="cart" />
</menu>

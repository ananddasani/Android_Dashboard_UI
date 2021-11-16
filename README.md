# Android_Dashboard_UI
A Dashboard UI App

# App Highlight

<img src="app_images/Dashboard UI Code2.png" width="1000" /><br>

<img src="app_images/Dashboard UI Code.png" width="1000" /><br>

<img src="app_images/Dashboard UI App.png" width="300" /><br>


# Code

#### activity_main.xml
```
<ScrollView
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

<androidx.constraintlayout.widget.ConstraintLayout

    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <TextView
        android:id="@+id/tv"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="16dp"
        android:layout_marginTop="16dp"
        android:layout_marginEnd="16dp"
        android:fontFamily="@font/aclonica"
        android:text="Coding"
        android:textSize="48sp"
        app:layout_constraintEnd_toStartOf="@+id/imageView"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/textView4"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="16dp"
        android:layout_marginTop="8dp"
        android:text="TEN/ADD/351 Anand Dasani"
        app:layout_constraintEnd_toEndOf="@+id/tv"
        app:layout_constraintStart_toStartOf="@+id/tv"
        app:layout_constraintTop_toBottomOf="@+id/tv" />

    <ImageView
        android:id="@+id/imageView"
        android:layout_width="147dp"
        android:layout_height="142dp"
        android:layout_marginTop="32dp"
        android:layout_marginEnd="16dp"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:srcCompat="@drawable/coding" />

<!--    this is first menu-->
    <LinearLayout
        android:id="@+id/linearLayout"
        android:layout_width="0dp"
        android:layout_height="170dp"
        android:layout_marginTop="16dp"
        android:orientation="horizontal"
        android:padding="10dp"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/imageView">

        <androidx.cardview.widget.CardView
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_margin="5dp"
            android:layout_weight="1" >

            <RelativeLayout
                android:layout_width="match_parent"
                android:layout_height="match_parent">

                <ImageView
                    android:id="@+id/imageView2"
                    android:layout_width="100dp"
                    android:layout_height="80dp"
                    android:layout_centerHorizontal="true"
                    android:layout_centerVertical="false"
                    android:layout_marginTop="10dp"
                    app:srcCompat="@drawable/java" />

                <TextView
                    android:id="@+id/textView5"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_below="@id/imageView2"
                    android:layout_centerHorizontal="true"
                    android:layout_marginStart="10dp"
                    android:layout_marginTop="10dp"
                    android:layout_marginEnd="10dp"
                    android:layout_marginBottom="10dp"
                    android:text="JAVA"
                    android:textSize="20sp"
                    android:textStyle="bold|italic" />
            </RelativeLayout>
        </androidx.cardview.widget.CardView>

        <androidx.cardview.widget.CardView
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_margin="5dp"
            android:layout_weight="1" >

            <RelativeLayout
                android:layout_width="match_parent"
                android:layout_height="match_parent">

                <ImageView
                    android:id="@+id/imageView3"
                    android:layout_width="100dp"
                    android:layout_height="80dp"
                    android:layout_centerHorizontal="true"
                    android:layout_centerVertical="false"
                    android:layout_marginTop="10dp"
                    app:srcCompat="@drawable/cpp" />

                <TextView
                    android:id="@+id/textView6"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_below="@id/imageView3"
                    android:layout_centerHorizontal="true"
                    android:layout_marginStart="10dp"
                    android:layout_marginTop="10dp"
                    android:layout_marginEnd="10dp"
                    android:layout_marginBottom="10dp"
                    android:text="C++"
                    android:textSize="20sp"
                    android:textStyle="bold|italic" />
            </RelativeLayout>
        </androidx.cardview.widget.CardView>
    </LinearLayout>

<!--    this is second menu-->
    <LinearLayout
        android:id="@+id/linearLayout2"
        android:layout_width="0dp"
        android:layout_height="170dp"
        android:layout_marginTop="16dp"
        android:orientation="horizontal"
        android:padding="10dp"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/linearLayout">

        <androidx.cardview.widget.CardView
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_margin="5dp"
            android:layout_weight="1">

            <RelativeLayout
                android:layout_width="match_parent"
                android:layout_height="match_parent">

                <ImageView
                    android:id="@+id/imageView4"
                    android:layout_width="100dp"
                    android:layout_height="80dp"
                    android:layout_centerHorizontal="true"
                    android:layout_centerVertical="false"
                    android:layout_marginTop="10dp"
                    app:srcCompat="@drawable/html" />

                <TextView
                    android:id="@+id/textView7"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_below="@id/imageView4"
                    android:layout_centerHorizontal="true"
                    android:layout_marginStart="10dp"
                    android:layout_marginTop="10dp"
                    android:layout_marginEnd="10dp"
                    android:layout_marginBottom="10dp"
                    android:text="HTML"
                    android:textSize="20sp"
                    android:textStyle="bold|italic" />
            </RelativeLayout>
        </androidx.cardview.widget.CardView>

        <androidx.cardview.widget.CardView
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_margin="5dp"
            android:layout_weight="1">

            <RelativeLayout
                android:layout_width="match_parent"
                android:layout_height="match_parent">

                <ImageView
                    android:id="@+id/imageView5"
                    android:layout_width="100dp"
                    android:layout_height="80dp"
                    android:layout_centerHorizontal="true"
                    android:layout_centerVertical="false"
                    android:layout_marginTop="10dp"
                    app:srcCompat="@drawable/css" />

                <TextView
                    android:id="@+id/textView8"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_below="@id/imageView5"
                    android:layout_centerHorizontal="true"
                    android:layout_marginStart="10dp"
                    android:layout_marginTop="10dp"
                    android:layout_marginEnd="10dp"
                    android:layout_marginBottom="10dp"
                    android:text="CSS"
                    android:textSize="20sp"
                    android:textStyle="bold|italic" />
            </RelativeLayout>
        </androidx.cardview.widget.CardView>
    </LinearLayout>

<!--    this is third menu-->
    <LinearLayout
        android:id="@+id/linearLayout3"
        android:layout_width="0dp"
        android:layout_height="170dp"
        android:layout_marginTop="16dp"
        android:layout_marginBottom="16dp"
        android:orientation="horizontal"
        android:padding="10dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/linearLayout2">

        <androidx.cardview.widget.CardView
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_margin="5dp"
            android:layout_weight="1">

            <RelativeLayout
                android:layout_width="match_parent"
                android:layout_height="match_parent">

                <ImageView
                    android:id="@+id/imageView6"
                    android:layout_width="100dp"
                    android:layout_height="80dp"
                    android:layout_centerHorizontal="true"
                    android:layout_centerVertical="false"
                    android:layout_marginTop="10dp"
                    app:srcCompat="@drawable/js" />

                <TextView
                    android:id="@+id/textView9"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_below="@id/imageView6"
                    android:layout_centerHorizontal="true"
                    android:layout_marginStart="10dp"
                    android:layout_marginTop="10dp"
                    android:layout_marginEnd="10dp"
                    android:layout_marginBottom="10dp"
                    android:text="JS"
                    android:textSize="20sp"
                    android:textStyle="bold|italic" />
            </RelativeLayout>
        </androidx.cardview.widget.CardView>

        <androidx.cardview.widget.CardView
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_margin="5dp"
            android:layout_weight="1">

            <RelativeLayout
                android:layout_width="match_parent"
                android:layout_height="match_parent">

                <ImageView
                    android:id="@+id/imageView7"
                    android:layout_width="100dp"
                    android:layout_height="80dp"
                    android:layout_centerHorizontal="true"
                    android:layout_centerVertical="false"
                    android:layout_marginTop="10dp"
                    app:srcCompat="@drawable/python" />

                <TextView
                    android:id="@+id/textView10"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_below="@id/imageView7"
                    android:layout_centerHorizontal="true"
                    android:layout_marginStart="10dp"
                    android:layout_marginTop="10dp"
                    android:layout_marginEnd="10dp"
                    android:layout_marginBottom="10dp"
                    android:text="PYTHON"
                    android:textSize="20sp"
                    android:textStyle="bold|italic" />
            </RelativeLayout>
        </androidx.cardview.widget.CardView>
    </LinearLayout>
</androidx.constraintlayout.widget.ConstraintLayout>

</ScrollView>
```

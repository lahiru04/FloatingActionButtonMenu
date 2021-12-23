# floatingx
Floating button menu library


<p align="center">
<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-brightgreen.svg" alt="License: MIT"></a>
<a href="https://jitpack.io/#lahiru04/floatingx"><img src="https://jitpack.io/v/lahiru04/floatingx.svg" alt="JitPack Build: Passing"></a>
</p>

## Installation

You can install this with [Gradle](#gradle) , [Maven](#maven) , [sbt](#sbt) or [Leiningen](#leiningen)

### Gradle

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  
  
    dependencies {
	        implementation 'com.github.lahiru04:floatingx:v1.0.0'
	}
  
### Maven

    <repositories>
		<repository>
		    <id>jitpack.io</id>
		    <url>https://jitpack.io</url>
		</repository>
	</repositories>
	
	<dependency>
    	    <groupId>com.github.lahiru04</groupId>
    	    <artifactId>floatingx</artifactId>
    	    <version>v1.0.0</version>
    </dependency>
    
 ### sbt    
    resolvers += "jitpack" at "https://jitpack.io"
    
    libraryDependencies += "com.github.lahiru04" % "floatingx" % "v1.0.0"	
    
 ### Leiningen
 
      :repositories [["jitpack" "https://jitpack.io"]]
      
      :dependencies [[com.github.lahiru04/floatingx "v1.0.0"]]	  
      
      
 ## Requirements
 
 <p>The library requires Android API Level 14+</p>     
 
 ## Sample
 
 ![Main screen](/motion1.gif)
 
 
 ## Usage
 
    <com.religious.floatingx.FloatingActionMenu
            android:id="@+id/menu"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="bottom|right"
            android:layout_marginRight="@dimen/fab_margin"
            android:layout_marginBottom="@dimen/fab_margin"
            app:menu_colorNormal="@color/colorPrimary"
            app:menu_colorPressed="@color/colorPrimary1"
            app:menu_colorRipple="@color/black">

            <com.religious.floatingx.FloatingActionButtonx
                android:id="@+id/fabSalesOrder"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                app:fab_colorNormal="@color/colorPrimary"
                app:fab_label="Sales Order"
                app:srcCompat="@drawable/ic_baseline_order_24" />

            <com.religious.floatingx.FloatingActionButtonx
                android:id="@+id/fabPendingOrder"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:visibility="gone"
                app:fab_colorNormal="@color/colorPrimary"
                app:fab_label="Pending Order"
                app:srcCompat="@drawable/ic_baseline_order_24" />


            <com.religious.floatingx.FloatingActionButtonx
                android:id="@+id/fabInvoice"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                app:fab_colorNormal="@color/colorPrimary"
                app:fab_label="Invoice"
                app:srcCompat="@drawable/ic_baseline_order_24" />

            <com.religious.floatingx.FloatingActionButtonx
                android:id="@+id/fabReturnNote"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                app:fab_colorNormal="@color/colorPrimary"
                app:fab_label="Return Note"
                app:srcCompat="@drawable/ic_baseline_remove_shopping_cart_24" />

            <com.religious.floatingx.FloatingActionButtonx
                android:id="@+id/fabUnproductive"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                app:fab_colorNormal="@color/colorPrimary"
                app:fab_label="Unproductive"
                app:srcCompat="@drawable/ic_baseline_unproductive_24" />

            <com.religious.floatingx.FloatingActionButtonx
                android:id="@+id/fabPosm"
                android:layout_width="wrap_content"
                android:visibility="gone"
                android:layout_height="wrap_content"
                app:fab_colorNormal="@color/colorPrimary"
                app:fab_label="POSM"
                app:srcCompat="@drawable/ic_baseline_posm_24" />

            <com.religious.floatingx.FloatingActionButtonx
                android:id="@+id/fabmMrchandising"
                android:layout_width="wrap_content"
                android:visibility="gone"
                android:layout_height="wrap_content"
                app:fab_colorNormal="@color/colorPrimary"
                app:fab_label="Merchandising"
                app:srcCompat="@drawable/ic_baseline_merchandise_24" />

            <com.religious.floatingx.FloatingActionButtonx
                android:id="@+id/fabCompetitorAnalysis"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                app:fab_colorNormal="@color/colorPrimary"
                app:fab_label="Competitor Analysis"
                app:srcCompat="@drawable/ic_baseline_directions_run_24" />

            <com.religious.floatingx.FloatingActionButtonx
                android:id="@+id/fabAddGondola"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                app:fab_colorNormal="@color/colorPrimary"
                app:fab_label="Add Gondola"
                app:srcCompat="@drawable/ic_baseline_gondola_24" />

        </com.religious.floatingx.FloatingActionMenu>
 

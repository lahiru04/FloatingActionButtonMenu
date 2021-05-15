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
 
    <com.github.clans.fab.FloatingActionMenu
         android:id="@+id/menu"
         android:layout_width="wrap_content"
         android:layout_height="wrap_content"
         android:layout_alignParentBottom="true"
         android:layout_alignParentRight="true"
         android:layout_marginRight="10dp"
         android:layout_marginBottom="10dp"
         android:layout_marginLeft="10dp"
         fab:menu_fab_size="normal"
         fab:menu_showShadow="true"
         fab:menu_shadowColor="#66000000"
         fab:menu_shadowRadius="4dp"
         fab:menu_shadowXOffset="1dp"
         fab:menu_shadowYOffset="3dp"
         fab:menu_colorNormal="#DA4336"
         fab:menu_colorPressed="#E75043"
         fab:menu_colorRipple="#99FFFFFF"
         fab:menu_animationDelayPerItem="50"
         fab:menu_icon="@drawable/fab_add"
         fab:menu_buttonSpacing="0dp"
         fab:menu_labels_margin="0dp"
         fab:menu_labels_showAnimation="@anim/fab_slide_in_from_right"
         fab:menu_labels_hideAnimation="@anim/fab_slide_out_to_right"
         fab:menu_labels_paddingTop="4dp"
         fab:menu_labels_paddingRight="8dp"
         fab:menu_labels_paddingBottom="4dp"
         fab:menu_labels_paddingLeft="8dp"
         fab:menu_labels_padding="8dp"
         fab:menu_labels_textColor="#FFFFFF"
         fab:menu_labels_textSize="14sp"
         fab:menu_labels_cornerRadius="3dp"
         fab:menu_labels_colorNormal="#333333"
         fab:menu_labels_colorPressed="#444444"
         fab:menu_labels_colorRipple="#66FFFFFF"
         fab:menu_labels_showShadow="true"
         fab:menu_labels_singleLine="false"
         fab:menu_labels_ellipsize="none"
         fab:menu_labels_maxLines="-1"
         fab:menu_labels_style="@style/YourCustomLabelsStyle"
         fab:menu_labels_position="left"
         fab:menu_openDirection="up"
         fab:menu_backgroundColor="@android:color/transparent"
         fab:menu_fab_label="your_label_here"
         fab:menu_fab_show_animation="@anim/my_show_animation"
         fab:menu_fab_hide_animation="@anim/my_hide_animation">
 
         <com.github.clans.fab.FloatingActionButton
             android:id="@+id/menu_item"
             android:layout_width="wrap_content"
             android:layout_height="wrap_content"
             android:src="@drawable/ic_star"
             fab:fab_size="mini"
             fab:fab_label="Menu item 1" />
 
     </com.github.clans.fab.FloatingActionMenu>
 
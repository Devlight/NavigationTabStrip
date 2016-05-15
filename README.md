
NavigationTabStrip
==================

Navigation tab strip with smooth interaction.

![](https://lh6.googleusercontent.com/-wpGnxe1Vefc/VziiygaS9WI/AAAAAAAACd4/c4fU_EG-DHkoby1SIbI5BDtqITpGiZZhwCL0B/w326-h551-no/nts.gif)

U can check the sample app [here](https://github.com/DevLight-Mobile-Agency/NavigationTabStrip/tree/master/app).

Download
------------

You can download a .aar` from GitHub's [releases page](https://github.com/DevLight-Mobile-Agency/NavigationTabStrip/releases).

Or use Gradle jCenter:

```groovy
dependencies {
    repositories {
        mavenCentral()
        maven {
            url  'http://dl.bintray.com/gigamole/maven/'
        }
    }
    compile 'com.github.devlight.navigationtabstrip:library:+'
}
```

Or Gradle Maven Central:

```groovy
compile 'com.github.devlight.navigationtabstrip:library:1.0.0'
```

Or Maven:

```groovy
<dependency>
    <groupId>com.github.devlight.navigationtabstrip</groupId>
    <artifactId>library</artifactId>
    <version>1.0.0</version>
    <type>aar</type>
</dependency>
```

Android SDK Version
=========

NavigationTabStrip requires a minimum SDK version of 11. 

Sample
========

For NTS you can set such parameters as:
 
 - color:
    
    allows you to set strip color.
    
 - size:
     
    allows you to set titles size. By default NTS use auto titles size.
    
 - weight:
     
    allows you to set weight(height) of strip.
    
 - factor:
     
    allows you to set strip resize factor.
    
 - titles:
    
    allows you to set NTS titles. This is your tabs.
    
 - type:
    
    allows you to set strip type - line or point.
    
 - gravity:
    
    allows you to set strip gravity - top or bottom.
    
 - view pager:
     
    allows you to connect NTS with ViewPager. If you want your can also set OnPageChangeListener.    
    
 - typeface:
 
    allows you to set custom typeface to your titles.
 
 - corners radius:
    
    allows you to set corners radius of strip.

 - animation duration:
  
    allows you to set animation duration.
      
 - inactive color:

    allows you to set inactive titles color.
     
 - active color:
  
    allows you to set active title color.
     
 - tab strip listener:
  
    allows you to set listener which triggering on start or on end when you set tab index.

If your set ViewPager you can action down on active tab and do like drag.

NTS use only upper case titles.

Check out in code init:

```java
final NavigationTabStrip navigationTabStrip = (NavigationTabStrip) findViewById(R.id.nts);
navigationTabStrip.setTitles("Nav", "Tab", "Strip");
navigationTabStrip.setTabIndex(0, true);
navigationTabStrip.setTitleSize(15);
navigationTabStrip.setStripColor(Color.RED);
navigationTabStrip.setStripWeight(6);
navigationTabStrip.setStripFactor(2);
navigationTabStrip.setStripType(NavigationTabStrip.StripType.LINE);
navigationTabStrip.setStripGravity(NavigationTabStrip.StripGravity.BOTTOM);
navigationTabStrip.setTypeface("fonts/typeface.ttf");
navigationTabStrip.setCornersRadius(3);
navigationTabStrip.setAnimationDuration(300);
navigationTabStrip.setInactiveColor(Color.GRAY);
navigationTabStrip.setActiveColor(Color.WHITE);
navigationTabStrip.setOnPageChangeListener(...);
navigationTabStrip.setOnTabStripSelectedIndexListener(...);
```
            
Other methods check out in sample.

And XML init:

```xml
<com.gigamole.library.NavigationTabStrip
    android:layout_width="match_parent"
    android:layout_height="50dp"
    app:nts_color="#000"
    app:nts_size="15sp"
    app:nts_weight="3dp"
    app:nts_factor="2.5"
    app:nts_titles="@array/titles"
    app:nts_type="point"
    app:nts_gravity="top"
    app:nts_typeface="fonts/typeface.otf"
    app:nts_corners_radius="1.5dp"
    app:nts_animation_duration="300"
    app:nts_active_color="#000"
    app:nts_inactive_color="#c4c4c4"/>
```

Getting Help
======

To report a specific problem or feature request, [open a new issue on Github](https://github.com/DevLight-Mobile-Agency/NavigationTabStrip/issues/new).

License
======

Apache 2.0 and MIT. See [LICENSE](https://github.com/DevLight-Mobile-Agency/NavigationTabStrip/blob/master/LICENSE.txt) file for details.

Inspiration
======

Original interaction | Point interaction | Line interaction
:-------------------------:|:-------------------------:|:-------------------------:
![](https://d7natbl5lhry0.cloudfront.net/media/resource_image/image_1506)|![](https://s-media-cache-ak0.pinimg.com/originals/42/b4/47/42b447c201642b2e82c981bc6599d850.gif)|![](https://s-media-cache-ak0.pinimg.com/originals/40/ae/5e/40ae5eed129a90ac9e7ee73cdb24e69d.gif)

Author
=======

Made in [DevLight Mobile Agency](https://github.com/DevLight-Mobile-Agency)

Created by [Basil Miller](https://github.com/GIGAMOLE) - [@gigamole](mailto:gigamole53@gmail.com)
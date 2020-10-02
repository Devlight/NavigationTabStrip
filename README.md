<br/>
<p align="center">
  <a href="http://devlight.io">
      <img src ="https://drive.google.com/uc?export=download&id=0BxPO_UeS7wScLVBKck51Z1Rzb0E" alt="Devlight"/>
  </a>
</p>
<br/>

NavigationTabStrip
==================

Navigation tab strip with smooth interaction.

[![Android Arsenal](https://drive.google.com/uc?export=download&id=0BxPO_UeS7wScN3B6NjFmWDVKaVE)](http://android-arsenal.com/details/1/3603)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Android](https://drive.google.com/uc?export=download&id=0BxPO_UeS7wSccEZaclNGN0R5OWc)](https://github.com/DevLight-Mobile-Agency)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Download](https://drive.google.com/uc?export=download&id=0BxPO_UeS7wScdFUzeWFwUURBME0)](https://bintray.com/gigamole/maven/navigationtabstrip/_latestVersion)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![License](https://drive.google.com/uc?export=download&id=0BxPO_UeS7wScU0tmeFpGMHVWNWs)](https://github.com/DevLight-Mobile-Agency/NavigationTabStrip/blob/master/LICENSE.txt)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Codacy](https://drive.google.com/uc?export=download&id=0BxPO_UeS7wScSHhmckZyeGJDcXc)](https://www.codacy.com/app/gigamole53/NavigationTabStrip?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=DevLight-Mobile-Agency/NavigationTabStrip&amp;utm_campaign=Badge_Grade)

<br/>

<p align="center">
  <img src ="https://drive.google.com/uc?export=download&id=0BxPO_UeS7wScR3FUNTRvS1BJeEE" alt="Devlight"/>
</p>

You can check the sample app [here](https://github.com/DevLight-Mobile-Agency/NavigationTabStrip/tree/master/app).

Warn
====
```
This library is not more supported. 
If you want to add new feature or fix a bug, grab source code and do it. 
If you think your fix or feature would be useful to other developers, 
I can add link of your repository to this README file. 
Thank you for using our libraries.
```

Download
========

You can download a `.aar` from GitHub's [releases page](https://github.com/DevLight-Mobile-Agency/NavigationTabStrip/releases).

Or use Gradle jCenter:

```groovy
dependencies {
    repositories {
        mavenCentral()
        maven {
            url  'http://dl.bintray.com/gigamole/maven/'
        }
    }
    implementation 'com.github.devlight.navigationtabstrip:navigationtabstrip:+'
}
```

Or Gradle Maven Central:

```groovy
compile 'com.github.devlight.navigationtabstrip:navigationtabstrip:1.0.4'
```

Or Maven:

```groovy
<dependency>
    <groupId>com.github.devlight.navigationtabstrip</groupId>
    <artifactId>navigationtabstrip</artifactId>
    <version>1.0.4</version>
    <type>aar</type>
</dependency>
```

Android SDK Version
===================

`NavigationTabStrip` requires a minimum SDK version of 11. 

Sample
======

<b>Parameters</b>

For `NTS` you can set such parameters as:
 
 - color:  
    allows you to set strip color.
    
 - size:  
    allows you to set titles size. By default `NTS` use auto titles size.
    
 - weight:  
    allows you to set weight(height) of strip.
    
 - factor:  
    allows you to set strip resize factor.
    
 - titles:  
    allows you to set `NTS` titles. This is your tabs.
    
 - type:  
    allows you to set strip type - line or point.
    
 - gravity:  
    allows you to set strip gravity - top or bottom.
    
 - view pager:  
    allows you to connect `NTS` with `ViewPager`. If you want your can also set `OnPageChangeListener`.    
    
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

<b>Tips</b>

If your set `ViewPager` you can action down on active tab and do like drag.  
`NTS` use only upper case titles.

<b>Init</b>

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
<com.gigamole.navigationtabstrip.NavigationTabStrip
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
============

To report a specific problem or feature request, [open a new issue on Github](https://github.com/DevLight-Mobile-Agency/NavigationTabStrip/issues/new).

Xamarin
=======

Thanks to [Martijn van Dijk](https://github.com/martijn00) for developing Xamarin bindings library for [NavigationTabStrip](https://github.com/martijn00/NavigationTabStripXamarin).  
Plugin is available on [Nuget](https://www.nuget.org/packages/Xam.Plugins.Android.NavigationTabStrip/).


Credits
=======

|[Keren Rijensky](https://dribbble.com/KerenRij)|[Srikant Shetty](https://dribbble.com/Srikant)|[Oleg Frolov](https://dribbble.com/Volorf)|
|:---------------------------------------------:|:--------------------------------------------:|:----------------------------------------:|
|[![](https://d13yacurqjgara.cloudfront.net/users/259538/screenshots/2594107/tabs-transition.gif)](https://dribbble.com/shots/2594107-tabs-transition)|[![](https://s-media-cache-ak0.pinimg.com/originals/42/b4/47/42b447c201642b2e82c981bc6599d850.gif)](https://dribbble.com/shots/2125041-Tab-interaction)|[![](https://s-media-cache-ak0.pinimg.com/originals/40/ae/5e/40ae5eed129a90ac9e7ee73cdb24e69d.gif)](https://dribbble.com/shots/2561589-Tabs)|

Author
======

Created by [Basil Miller](https://github.com/GIGAMOLE) - [@gigamole](mailto:gigamole53@gmail.com)

Company
=======

[![Facebook](https://drive.google.com/uc?export=download&id=0BxPO_UeS7wScaGhGVFNKU0VxMnc)](https://www.facebook.com/devlightagency)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Twitter](https://drive.google.com/uc?export=download&id=0BxPO_UeS7wScZ1ExQWh5cHF5cVE)](https://twitter.com/DevLightIO)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![LinkedIn](https://drive.google.com/uc?export=download&id=0BxPO_UeS7wSccGZINzEycE1nVFE)](https://www.linkedin.com/company/devlight)

[Here](https://github.com/DevLight-Mobile-Agency) you can see open source work developed by Devlight LLC.  
This and another works is an exclusive property of Devlight LLC. 

If you want to use this library in applications which will be available on Google Play, please report us about it or author of the library.

Whether you're searching for a new partner or trusted team for creating your new great product we are always ready to start work with you. 

You can contact us via info@devlight.io or opensource@devlight.io.  
Thanks in advance.

Devlight LLC, 2016  
[devlight.io](http://devlight.io) 

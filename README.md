android-OverscrollViewPager
=====

android-OverscrollViewPager is an extension of ViewPager provided with a `overscroll` behavior callback along with a orientation property.
Screenshot
--------
![](http://ww3.sinaimg.cn/large/7adcb3b9gw1f1wx0i5vnbg20qo1bfdt0.gif)
Download
--------
Gradle:

```gradle
repositories {
  mavenCentral() // jcenter() works as well because it pulls from Maven Central
}

dependencies {
  compile 'me.linshen.overscrollviewpager:library:1.0.1'
}
```

Or Maven:

```xml
<dependency>
  <groupId>me.linshen.overscrollviewpager</groupId>
  <artifactId>library</artifactId>
  <version>1.0.1</version>
  <type>pom</type>
</dependency>
```

How do I use OverscrollViewPager?
-------------------
Import in your xml layout file:

```xml
<me.linshen.android.widget.OverScrollViewPager
        android:id="@+id/vp"
        android:layout_width="match_parent"
        android:layout_height="match_parent" />
```        

Find it in your Activity or Fragment

```java
// For a simple view:
mViewPager = (OverScrollViewPager) findViewById(R.id.vp);
```

Add a listener to it

```java
mViewPager.addOnPageOverScrollListener(new OverScrollViewPager.OnPageOverScrollListener() {
   @Override
   public void onPageOverScrolled(OverScrollViewPager.SCROLL_STATE state) {
           //TODO make your own behavior here  
       }
   });
```

Samples
-------
See `app` module in this project

License
-------
Copyright (C) 2016 Shen Lin

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.



Infinite ViewPager With Indicator
===============
A lightweight infinite viewpager indicator

![InfiniteViewPagerWithIndicator](/screenshot.gif)

Usage
--------
```xml
    <com.antonyt.infiniteviewpager.InfiniteViewPager
        android:id="@+id/viewpager"
        android:layout_width="match_parent"
        android:layout_height="match_parent" />

    <me.relex.circleindicator.CircleIndicator
        android:id="@+id/indicator"
        android:layout_width="match_parent"
        android:layout_height="48dp" />
```
Wrap your existing PagerAdapter with the `InfinitePagerAdapter`:

```Java
	PagerAdapter wrappedAdapter = new InfinitePagerAdapter(adapter);
	viewPager.setAdapter(wrappedAdapter);
```

#####Properties For `CircleIndicator`:

* `app:ci_width`
* `app:ci_height`
* `app:ci_margin`
* `app:ci_drawable`
* `app:ci_drawable_unselected`
* `app:ci_animator`
* `app:ci_animator_reverse`

# Installing

Step 1:Add the JitPack repository to your build file
```gradle
allprojects {
		repositories {
			...
			maven { url "https://jitpack.io" }
		}
	}
```

Step 2:Add the dependency
```gradle
dependencies {
	compile 'com.github.hanihashemi:InfiniteViewPagerWithIndicator:1.1.8'
}
```
License
--------
```
Copyright (C) 2014 relex

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

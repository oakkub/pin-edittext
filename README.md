# pin-edittext

[![platform](https://img.shields.io/badge/platform-android-brightgreen.svg)](https://www.android.com)
[![API](https://img.shields.io/badge/API-15%2B-brightgreen.svg?style=flat)](https://img.shields.io/badge/platform-android-brightgreen.svg)
[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg?style=flat)](https://www.apache.org/licenses/LICENSE-2.0.html)

An extension of EditText with pin style

![Sceenshot](https://user-images.githubusercontent.com/9587882/31598644-f307ce54-b278-11e7-8082-34249a4e07c5.gif)

Usage
--------
Include `PinCodeEditText` in your layout XML
```xml
<com.oakkub.android.PinEditText
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:maxLength="4"
    android:inputType="textNoSuggestions"
    app:pinHighlightStateDrawable="@drawable/pin_oval_highlight_state"
    app:pinNormalStateDrawable="@drawable/pin_oval_normal_state"
    app:pinSpace="16dp"
    app:pinHeight="24dp"
    app:pinWidth="24dp"/>
```
- **android:maxLength:** The total pin **(Required to make PinEditText limit its length)**
- **android:inputType:** Preferred "textNoSuggestions" (If you want text) or "number" (If you want only number)
- **app:pinSpace:** Space between each pin (Default: 16dp)
- **app:pinHeight:** Height of each pin (Default: 24dp)
- **app:pinWidth:** Width of each pin (Default: 24dp)
- **app:pinHighlightStateDrawable:** Drawable of each pin that already has text
- **app:pinNormalStateDrawable:** Drawable of each empty pin

Requirement
--------
Android API 15 or higher

Download
--------
Add this to your app module's `build.gradle` file 
```groovy
dependencies {
    ...
    compile 'com.oakkub.android:pin-edittext:1.1.2'
}
```

License
--------

    Copyright 2017

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

<h1>
GoogleMap

<a href="https://console.developers.google.com/flows/enableapi?apiid=maps_android_backend&keyType=CLIENT_SIDE_ANDROID&r=88:96:69:E3:0A:F9:78:D8:82:15:09:6E:F3:0E:E6:EE:96:A9:7A:2A%3Bcom.hsnlearning.mymap">Click here for get Api Key </a>


--------------------
Enable 3 things...
Places Api
MapEmbaded Api 
Map javascript Api

Must watch this video for this..
https://www.youtube.com/watch?v=LEz6F04vRTQ&feature=youtu.be

---------------------------------------------------------
Magic Button


<br.com.bloder.magic.view.MagicButton
        android:id="@+id/magic_button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:magic_button_size="50dp"
        app:button_icon="@drawable/your_icon"
        app:button_icon_width="25dp"
        app:button_icon_height="25dp"
        app:hide_text="Hi Mom!"
        app:hide_text_size="15dp"
        app:hide_text_color="@android:color/black"
        app:icon_button_color="button_icon_color"
        app:expandable_area_color="that_expandable_button_part_color"/>
        
How about click event?
In magic button, the click event will work only in second click and you can set this event with:

magicButton.setMagicButtonClickListener(new View.OnClickListener() {
      @Override
      public void onClick(View v) {
        yourAction();
      }
});
Import
Gradle
dependencies {
    compile 'com.github.bloder:magic:1.1'
}
Maven
<dependency>
  <groupId>com.github.bloder</groupId>
  <artifactId>magic</artifactId>
  <version>1.1</version>
  <type>pom</type>
</dependency>
Ivy
<dependency org='com.github.bloder' name='magic' rev='1.1'>
  <artifact name='$AID' ext='pom'></artifact>
</dependency>
License
The MIT License (MIT)

Copyright (c) 2016 Bloder

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
------------------------------------------
Elegant Number Button
A simple Android library to implement a number counter with increment and decrement buttons.

 

Download
Grab the latest version on gradle using

compile 'com.cepheuen.elegant-number-button:lib:1.0.2'
or on maven

<dependency>
  <groupId>com.cepheuen.elegant-number-button</groupId>
  <artifactId>lib</artifactId>
  <version>1.0.2</version>
  <type>pom</type>
</dependency>

Usage
For Working implementation of this library check ElegantNumberButtonSample App

Just include the view as you do with any android widget.

Implement it in your java code as anyother widget.

To get the number simply call getNumber() method on the button object.

To get the number from the button as soon as the button is clicked add a setOnClickListener to the view.

ElegantNumberButton button = (ElegantNumberButton) findViewById(R.id.button);
button.setOnClickListener(new ElegantNumberButton.OnClickListener() {
        @Override
        public void onClick(View view) {
            String num = button.getNumber();
        }
    });
Or use a valueChangeListener to listen for changes in value.

elegantNumberButton.setOnValueChangeListener(new ElegantNumberButton.OnValueChangeListener() {
        @Override
        public void onValueChange(ElegantNumberButton view, int oldValue, int newValue) {
            Log.d(TAG, String.format("oldValue: %d   newValue: %d", oldValue, newValue));
        }
    });
Customization
backgroundColor : Set button Background color

initialNumber: Set initial number for the button.

finalNumber : Set final number range for button.

textColor: Modify the text color of the button.

textSize: Change text size of the button.

backgroundDrawable: Add drawable background for the button.

Methods
setNumber(Integer number): Update the number of the widget.

setRange(Integer startNumber, Integer finalNumber) : Set the operational range for the widget

setOnValueChangeListener(OnValueChangedListener listener): listen for changes in the value

Contributing
Fork it!
Create your feature branch: git checkout -b my-new-feature
Commit your changes: git commit -am 'Add some feature'
Push to the branch: git push origin my-new-feature
Submit a pull request
Changelog
Version 1.0.2
Added ValueChangeListener to listen for changes in values
Version 1.0.1
Added Range for the widget
Changed attribute from initialText to initialNumber
Version 1.0
Initial Release
Author
Hassanarshad.bwn@gmail.com
License
Copyright 2016 Hassan Arshad

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

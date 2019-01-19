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
alt tag

What is Magic Button?
It's a new button in android that hypnotizes the user and make him give you a lot of money!!! 
Ok, just kidding, this is not so magic yet... but it's a cute button. 



alt tag 

Ok it's cute, But how can I use
You just need to add this in your layout.

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

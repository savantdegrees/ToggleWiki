#### Example
Below shows an example of section title.

~~~html
<div class="section-header neutral">
 <div class="wrap">
  <div class="section-header__outer">
   <div class="section-header__title">
    <span><a href="#"><i class="i-channelu--st"></i>Parent Section Title Name Lorem Ipsum</a></span>
    <span><a href="#" data-dotdot="1">Current Section Title Name Lorem Ipsum</a></span>
   </div>
  </div>
 </div>
</div>
~~~

#### Titles
A maximum of 2 titles can be used.  A title is defined by

~~~html
 <span><a href="#"><i class="i-channelu--st"></i>Parent Section Title Name Lorem Ipsum</a></span>
~~~

If only 1 span title is used, it is automatically defaulted as the current section title and use the appropriate styling.

If 2 span titles are used, the first title is defaulted as parent section title, and the second title is defaulted as current section title

Any icons can be added to the title, using the `<i class="i-icon-name"></i>`.  Icon should be placed within the anchor element so it is part of the clickable title.

#### Visual Modifiers
`.neutral` adds a neutral black background color when icons are used.  This is an optional class that can be used when author feels background makes icon too visually busy.


#### Customizing the Background Colors And Images
Current colors are now fixed in the thematic styles.  You can overwrite the current background colors and images with the following code.  For microsites, we recommend putting them in a generated css file such as the `custom-microsite.css` file

To change the background color of the section header, overwrite the styles by
~~~html
.section-header {
 background: #my-new-color !important; //!important required since thematic styles have higher specificity
}
~~~

To add a new custom background color to the section header, overwrite the styles by 
~~~html
.section-header .section-header__outer {
 background-image: url("../../images/localnav/sechead-entertainment-bg.png"); //override this URL
}

@media screen and (min-width: 780px) {
 .section-header .section-header__outer {
  background-image: url("../../images/localnav/sechead-entertainment-bg.png"); //override this URL
  }
}
~~~

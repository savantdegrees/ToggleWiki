## Megaslider: 

The Megaslider is a very customisable component that allows you to have vastly different configurations on each page. 

There are 6 different types of megasliders that are configured within the Toggle project right now. 

The 6 types of Megasliders are: 

- `.megaslider`
- `.megaslider__single`
- `.megaslider__portrait`
- `.megaslider__8 `
- `.megaslider__8-3up`
- `.megaslider__4`

### Megaslider

The Megaslider must have the `.megaslider` class and uses a combination of the following megaslider items 

- {{> molecules-megaslider-item-featured }}
- {{> molecules-megaslider-ad-item }}
- {{> molecules-megaslider-three-items }}
- {{> molecules-megaslider-four-items }}

~~~html
<!-- Optional card class to add a card effect -->
<div class="megaslider-holder card">
  <h2>
    <!-- Optional image for channel icon -->
    <img src="../../images/icons-tvchannel/C5_36x36.png" alt="">
    <a href="#"> {{ slider-title }} <i class="ti-chevron-next"></i></a></h2>
  <div class="megaslider ">
    {{> molecules-megaslider-item-featured }}
    {{> molecules-megaslider-three-items }}
    {{> molecules-megaslider-ad-item }}
    {{> molecules-megaslider-four-items }}
    {{> molecules-megaslider-item-featured }}
    {{> molecules-megaslider-three-items }}
  </div>
</div>
~~~

**Note:** If megaslider is on the home page, it will have a colored border at the top. You can add the `theme class` to the `.megaslider-holder` to show the correct color. 

~~~html
<div class="megaslider-holder collapsible card {{class}}">
  // Other megaslider stuff
</div>
~~~


### Megaslider__single

The Megaslider__single must have the `.megaslider__single` class in addition to `.megaslider` and uses a combination of two megaslider items:

- {{> molecules-megaslider-item }}
- {{> molecules-megaslider-item-nowplaying }}

~~~html
<div class="megaslider-holder card">
  <h2><img src="../../images/icons-tvchannel/C5_36x36.png" alt=""><a href="#"> {{ megaslider-title }} <i class="ti-chevron-next"></i></a></h2>
  <div class="megaslider megaslider__single">
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item-nowplaying }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
  </div>
</div>
~~~
### Megaslider__portrait

The Megaslider__portrait must have the `.megaslider__portrait` class in addition to `.megaslider` and uses a combination only one megaslider item 

- {{> molecules-megaslider-item-portrait }}

~~~html
<div class="megaslider-holder card">
  <h2>
    <img src="../../images/icons-tvchannel/C5_36x36.png" alt="">
    <a href="#"> {{slider-title}} <i class="ti-chevron-next"></i></a>
  </h2>
  <div class="megaslider megaslider__portrait">
    {{> molecules-megaslider-item-portrait }}
    {{> molecules-megaslider-item-portrait }}
    {{> molecules-megaslider-item-portrait }}
    {{> molecules-megaslider-item-portrait }}
    {{> molecules-megaslider-item-portrait }}
    {{> molecules-megaslider-item-portrait }}
    {{> molecules-megaslider-item-portrait }}
    {{> molecules-megaslider-item-portrait }}
    {{> molecules-megaslider-item-portrait }}
    {{> molecules-megaslider-item-portrait }}
    {{> molecules-megaslider-item-portrait }}
    {{> molecules-megaslider-item-portrait }}
  </div>
</div>
~~~

### Megaslider__8 

The Megaslider__8 must have the `.megaslider__8` class in addition to `.megaslider` and uses a combination only one megaslider item 

- {{> molecules-megaslider-item }}

It is placed only in `.l-gi` of the 8 column content

~~~html
<div class="megaslider-holder card">
  <h2>{{slider-title}}</h2>
  <div class="megaslider megaslider__8">
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
  </div>
</div>
~~~

### Megaslider__8--3up

The Megaslider__8--3up must have the `.megaslider__8--3up` class in addition to `.megaslider` and uses a combination only one megaslider item. 

- {{> molecules-megaslider-item }}

It is placed only in `.l-gi` of the 8 column content. It contains 3 megaslider items in the 8 column content instead of 2.

~~~html
<div class="megaslider-holder card">
  <h2>{{slider-title}}</h2>
  <div class="megaslider megaslider__8--3up">
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
  </div>
</div>
~~~

### Megaslider__4

The Megaslider__4 must have the `.megaslider__4` class in addition to `.megaslider` and uses a combination only one megaslider item. 

- {{> molecules-megaslider-item }}

It is placed only in `.l-gi` of the 4 column content. It only shows one megaslider item at a time. 

~~~html
<div class="megaslider-holder card">
  <h2>{{ slider-title }}</h2>
  <div class="megaslider megaslider__4 card">
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
    {{> molecules-megaslider-item }}
  </div>
</div>
~~~

Custom Megaslider initialization 

If you want to do your own Custom Megaslider initialisation, add in your own megaslider and initialise it within init.js

## Megaslider Items
There are 7 kinds of megaslider items, all of them are combinations of either the [toggle teaser item]() or the [toggle list item]().  

- megaslider-item
- megaslider-item-portrait
- megaslider-item-featured
- megaslider-item-nowplaying
- megaslider-three-items
- megaslider-four-items
- megaslider-ad-item

### Megaslider-item
~~~html
<div class="megaslider__item">
  {{> toggle-teaser-item }} 
</div>
~~~

### Megaslider-item-portrait

~~~html
<div class="megaslider__item">
  {{> toggle-teaser-item-portrait }} 
</div>
~~~

### Megaslider-item-featured

~~~html 
<div class="megaslider__item">
  {{> toggle-teaser-item }} <!-- featured: true--> 
</div>
~~~

### Megaslider-item-nowplaying

~~~html
<div class="megaslider__item">
  {{> toggle-teaser-item }} <!-- now playing: true--> 
</div>
~~~

### Megaslider-three-items

~~~html
<div class="megaslider__item megaslider__item--3">
  {{> toggle-list-item }}
  {{> toggle-list-item }}
  {{> toggle-list-item }}
</div>
~~~

### Megaslider-four-items

~~~html
<div class="megaslider__item megaslider__item--4">
  {{> toggle-teaser-item }}
  {{> toggle-teaser-item }}
  {{> toggle-teaser-item }}
  {{> toggle-teaser-item }}
</div>
~~~

### Megaslider-ad-item

~~~html
<div class="megaslider__item megaslider__item--1">
  {{> ad-300x250-block }}
</div>
~~~

## Combinations of Megaslider Items 

### Double Slider (with Featured) 

~~~html
<div class="megaslider-holder card">
  <h2>
    <img src="../../images/icons-tvchannel/C5_36x36.png" alt="">
    <a href="#"> {{ slider-title }} <i class="ti-chevron-next"></i></a>
  </h2>
  <div class="megaslider card">
    {{> megaslider-item-featured }}
    {{> megaslider-four-items }}
    {{> megaslider-four-items }}
    {{> megaslider-four-items }}
    {{> megaslider-four-items }}
    {{> megaslider-four-items }}
  </div>
</div>
~~~

### Double Slider (no featured) 

~~~html
<div class="megaslider-holder card">
  <h2>
    <img src="../../images/icons-tvchannel/C5_36x36.png" alt="">
    <a href="#"> {{ slider-title }} <i class="ti-chevron-next"></i></a>
  </h2>
  <div class="megaslider card">
    {{> megaslider-four-items }}
    {{> megaslider-four-items }}
    {{> megaslider-four-items }}
    {{> megaslider-four-items }}
    {{> megaslider-four-items }}
    {{> megaslider-four-items }}
  </div>
</div>
~~~
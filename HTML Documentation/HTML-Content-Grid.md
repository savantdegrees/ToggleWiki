## Content Grid

- `data-content-grid-type`= `2` | `3` | `4` (`2` if placed in 8 columns, `3` if placed in 12 columns, `4` if its like price plan)
- `data-rows-on-desktop` = number of rows (integer) of content on a desktop view (there are 2 items per row if `type = 2`, 3 items per row if `type = 3`). It is used to calculate how many items to show / hide on smaller viewports. Leave empty if everything has to be shown

~~~html
<!-- Content Grid-->
<div class="tg-content-grid card" data-content-grid-type="2" data-rows-on-desktop="{{ rows }}">
  <h2><a href="#">{{ component-title }}<i class="ti-chevron-next"></i></a></h2>
  <div class="l-content-grid" >
    <div class="l-gi"> {{> molecules-toggle-list-item}} </div>
    <div class="l-gi"> {{> molecules-toggle-list-item}} </div>
    <div class="l-gi"> {{> molecules-toggle-list-item}} </div>
    <div class="l-gi"> {{> molecules-toggle-list-item}} </div>
    <div class="l-gi"> {{> molecules-toggle-list-item}} </div>
    <div class="l-gi"> {{> molecules-toggle-list-item}} </div>
  </div>
  <a href="#" class="tg-load-more btn">Load More</a>
</div>
~~~

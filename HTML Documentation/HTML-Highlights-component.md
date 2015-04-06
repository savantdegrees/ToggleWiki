## Highlights 
~~~
<!-- highlights -->
<div class="tg-highlights-holder">
  <div class="tg-highlights card">
    <h5>{{highlights-title}}</h5>
    <div class="l-3up">
      {{> molecules-toggle-teaser-item(type: video)}}
      {{> molecules-toggle-teaser-item(type: video)}}
      {{> molecules-toggle-teaser-item(type: video, suggested: true)}}
    </div>
  </div>
  
  <!-- Note: MUST HAVE split-insert. This is used to insert the ad into the correct place on tablet and mobile screens --> 
  <div class="split-insert" data-split-index="0"></div>
</div>
<!--/end highlights -->

~~~
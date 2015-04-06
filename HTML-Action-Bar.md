## Action Bar 

~~~html
<!-- actionbar -->
<div class="tg-actionbar card">
  <div class="l-gi">
    {{> actionbar-item}} 
  </div>
  <div class="l-gi">
    {{> actionbar-item}} 
  </div>
</div>
<!-- /end actionbar -->
~~~

## Actionbar-item 

~~~html 
<div class="actionbar__item">
  <h5> 
    <!-- optional to have arrow or link -->
    <a href="#"> {{Actionbar Item Title}} 
      <i class="ti-chevron-next"></i>
    </a>
  </h5>
  {{> toggle-list-item}}  
</div>
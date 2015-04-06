## Split Grid 

Split grid allows you to move any component from the sidebar to the main content area. 
The requirements are: 

- origination div must have `.split-grid` class 
- target will be `.split-insert` div 
- `split-index` values of the component being moved from the originating div must be the same as the split index from the target div 

~~~html
<div class="l-2up--8-4">
  <div class="l-gi">
    <div class="split-insert" data-split-index="{{ split-index }}"></div>
  </div> 

  <div class="l-gi split-grid">
    <div data-split-index="{{ split-index }}">
  </div>
</div>
~~~
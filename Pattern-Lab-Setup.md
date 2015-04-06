## Installation & Setup

Here are the steps to set things up: 

1. Clone the git repo 
2. Install nodejs 
3. install grunt-cli - sudo npm install grunt-cli -g
4. install Sass - `sudo gem install sass`
5. Install susy - `sudo gem install susy`
6. run `npm install` in cloned git. 
7. install bower - `sudo npm install bower -g` 
8. install bower components - `bower install` 
9. run `grunt` and navigate to 0.0.0.0:9000 in your browser. 

IF Grunt doesn't work (Step 9 has an error): 

1. run `php core/builder.php -wr` in cloned git. 
2. Find a way to compile Sass to CSS (Terminal, codekit etc). 
3. If you use Terminal, run `sass --watch scss:css -r susy`
4. Open public/index.html


## Structures: 

- HTML files are stored as `.mustache` files and are found under `source` -> `patterns`. The folder will correspond to the top left folder. 
- SCSS files are stored in `source` -> `scss`. Most components are either stored in `element` or `components` folder. 
- JS files are stored in `source` -> `js`. They are included into the website through the file in `00-atoms`-> `00-meta` -> `01-foot.js`. 

## Scss Methodology used 

1. BEM method for naming convention. 
2. Mobile first media queries with breakpoint mixin. 
3. Themes styles use either 
    - toggle dominant color (tdc). 
    - toggle ui color(tui). 
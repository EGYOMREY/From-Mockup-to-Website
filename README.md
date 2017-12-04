# Project: from Mockup to Website

I took [this design](https://egyomrey.github.io/From-Mockup-to-Website/Dribbble%20mockup.jpg) from Dribbble.com and used Sass to build it as a website.

[DIRECT LINK](https://egyomrey.github.io/From-Mockup-to-Website/build/index.html)

## How this project was built:


### 1. Styling

- Done with Sass, complied and minified to css with [Gulp](https://gulpjs.com/)
- Followed a basic [7-1 Pattern](https://sass-guidelin.es/#the-7-1-pattern)

**Final Sass folder structure:**
 <pre>
sass/  
|  
|– abstracts/  
|   |– _variables.scss 
|   |– _mixins.scss
|  
|– base/  
|   |– _base.scss  
|   |– _typography.scss  
|  
|– components/  
|   |– _award-display.scss
|   |– _button.scss   
|   |– _footer-form.scss  
|   |– _offers-block.scss  
|   |– _service-block.scss  
|   |– _slogan.scss         
|  
|– layout/  
|   |– _grid.scss  
|   |– _header.scss
|   |– _navigation.scss         
|   |– _hero-section.scss       
|   |– _services-section.scss       
|   |– _awards-section.scss     
|   |– _articles-section.scss
|   |– _big-footer.scss
|   |– _footer-nav.scss     
|  
|– vendors/  
|   |– _normalize.scss   
|  
– main.scss           
 </pre>

### 2. Gulp plugins used:
 <pre>
    gulp = require('gulp'),
    sass = require('gulp-sass'),
    browserSync = require('browser-sync'),
    uglify = require('gulp-uglify'),
    concatify = require('gulp-concat'),
    sourcemaps = require('gulp-sourcemaps'),
    autoprefixer = require('gulp-autoprefixer'),
    htmlmin = require('gulp-htmlmin');
</pre>

### 3. Svg icons

Took the social svg from this repository: 
[Font-Awesome-SVG-PNG](https://github.com/encharm/Font-Awesome-SVG-PNG)

### 4. Compression

Pictures were compressed with [Compressor.io](https://compressor.io)

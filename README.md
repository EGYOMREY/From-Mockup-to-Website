# Project: from Mockup to Website

I took [this design](https://egyomrey.github.io/From-Mockup-to-Website/Dribbble%20mockup.jpg) from Dribbble.com and used Sass to build it as a website. [Try it out](https://egyomrey.github.io/From-Mockup-to-Website/build/index.html) :arrow_upper_right:

## Desktop
![image](https://i.imgur.com/e9HkQXr.png)

## Mobile
![image](https://i.imgur.com/ynLgF5A.png)


## How to use this project
- To **clone** this repository with Git type in your console `git clone https://github.com/EGYOMREY/Portfolio.git`
- You can also **download** the code by pressing the button **Clone or Download** and then **Download ZIP**

All the source code is in the `src` folder, the minified and compressed version is in the `build` folder

- To open it in your browser, go to the project's folder, then in the `build` folder execute the index.html file.

If you'd like to work on this project (and use Gulp), after downloading or cloning it, go to the project's folder location with your console and 

1. Type `npm install` so you can work with the dependencies I used for developing it. (wait for the installation to complete)
2. Type `gulp` in the console and a new browser window will open pointing to your `localhost:3000` 
3. You can start working with the files located in the `src` folder. Open it with your text editor.

Gulp will refresh the browser with any saved change done in `src`, and also will output the minified and compressed version in the `build` folder.

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

## Motivation
I liked this design which seemed challenging to build into a responsive design, and since most designs in dribbble.com don't bring a picture of the mobile design, I thought I could make a working design.

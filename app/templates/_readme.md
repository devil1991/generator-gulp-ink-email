# <%= name %>

> This is <%= name %> description 

## How to install

Prerequisites:
* [Node.js](http://nodejs.org/) >=0.10.0
* [Gulp.js](http://gulpjs.com/) >=3.8.0 
<% if (sass) { %>* [Sass](http://sass-lang.com/) >=3.4.0  <% } %>

Installation process:
1. Clone this repository
2. Run ```npm install``` to install dependencies

## Usage

For project development with livereload run:
```
gulp serve
```

To build project run: (Result will be in ```dist/``` folder.)
```
gulp build
```

To serve builded project:
```
gulp serve:dist
```

## Built-in features

* ZURB Ink responsive email templates
<% if (sass) { %>* ZURB Ink CSS using Sassy Ink [Unofficial Sass port of Ink, Zurb's responsive email framework](https://github.com/faustgertz/sassy-ink)<% } else { %>* ZURB Ink.css<% } %>
* Webserver with liverelaod
<% if (jade) { %>* Jade templates compilation<% } %>
<% if (sass) { %>* Sass compilation<% } %>
* CSS concating and inlining

## Notes

Media queries should be revisited, because all of them are inlined into head.

---

Project structure was generated by [generator-gulp-ink-email](https://github.com/lightingbeetle/generator-gulp-ink-email) using version <%= version %>.  
 
[![Lighting Beetle](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Lighting Beetle")](http://www.lbstudio.sk)
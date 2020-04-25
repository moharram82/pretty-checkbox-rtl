<h1 align="center">
  <br> <br> pretty-checkbox-rtl <br>
</h1>

<h4 align="center">A pure CSS library built on <a href="https://github.com/lokesh-coder/pretty-checkbox">
    pretty-checkbox.css
  </a> to beautify checkbox and radio buttons, with support for RTL languages.</h4>

<br>

### Features
* Basic
  - **Shapes** - *Square*, *Curve*, *Round* 
  - **Variants** - *Default*, *Fill*, *Thick*
  - **Colors** - *Primary*, *Success*, *Info*, *Warning*, *Danger* 
  - **Color types** - *Solid*, *Outline*
  - **Animations** - *Smooth*, *Tada*, *Jelly*, *Pulse*, *Rotate*
 * Switch - iOS style - *Outline*, *Fill*, *Slim*
 * Responsive
 * No JavaScript
 * Custom Font Icons
 * SVG Icons
 * Image support
 * Toggle between icons / SVG's / images
 * Lock
 * State - *Focus*, *Hover*, *Indeterminate*
 * Supports frameworks - *Bootstrap*, *Foundation*, *Sematic UI*, *Bulma*, ...
 * SCSS customization
 * Supports all modern browsers, including mobile devices
 * Print friendly
 * and more... ( *I am kidding, that's all!* )

### Installation
- **From CLI**

Install the library from [`npm`](https://www.npmjs.com/package/pretty-checkbox-rtl) package manager

```sh
> npm install @moharram82/pretty-checkbox-rtl
```
Add `pretty-checkbox.min.css` in your html

<br>

- **Manual download** ( [`Github`](https://github.com/moharram82/pretty-checkbox-rtl/archive/master.zip) )

Download the source from Github.
```html
<link rel="stylesheet" href="../<PATH>/pretty-checkbox-rtl/dist/pretty-checkbox.min.css"/>
```
`<PATH>` is where the library is downloaded.

<br>

**SCSS**

You can also import `pretty-checkbox.scss` in your main scss file.
```scss
@import '~pretty-checkbox-rtl/src/pretty-checkbox.scss';
```

Please refer the document for SCSS settings.


### Usage


Pretty checkbox comes with many styles,

| Class name  | Description              |
| :---------- | :----------------------- |
| `p-default` | Basic style              |
| `p-switch`  | iOS like toggle style    |
| `p-icon`    | Custom font icons        |
| `p-svg`     | Custom SVG files, markup |
| `p-image`   | Tiny images              |

And three shapes `p-round` `p-curve` `p-square` (default)


#### Basic checkbox

```html
  <div class="pretty p-default">
    <input type="checkbox" />
    <div class="state">
      <label>Check me</label>
    </div>
  </div>
```

Basic checkbox has three variants `p-fill` `p-thick` `p-outline` (default)

You can combine them.

```html
  <div class="pretty p-default p-curve p-fill">
    <input type="checkbox" />
    <div class="state">
      <label>Fill</label>
    </div>
  </div>
```

<div align="center"><strong >---</strong></div>

#### Switch checkbox

Switch has three variants `p-outline` `p-fill` `p-slim`

```html
  <div class="pretty p-switch p-fill">
    <input type="checkbox" />
    <div class="state">
      <label>On</label>
    </div>
  </div>
```

<div align="center"><strong >---</strong></div>

#### Custom Font icons

```html
  <div class="pretty p-icon">
    <input type="checkbox">
    <div class="state">
      <i class="icon fa fa-check"></i>
      <label>Check me</label>
    </div>
  </div>
```

<blockquote>
    <sub>
    	<strong>Note</strong>: class `icon` should be added along with icon class names
    </sub>
</blockquote>

<blockquote>
    <sub>
    	<strong>Note</strong>: For icons to work, you need to add appropriate font icons library. In above example , we used font awesome icon. So, FontAwesome should be included separately. 
    </sub>
</blockquote>

<div align="right">
 <i><sub><a href="https://lokesh-coder.github.io/pretty-checkbox#fonticons">
 more details</a></sub></i>
</div>

<div align="center"><strong >---</strong></div>

#### SVG

Supports SVG file in <img/> tag, markup (`<svg> ... </svg>`) and sprites  

```html
  <div class="pretty p-svg">
    <input type="checkbox">
    <div class="state">
      <img class="svg" src="file.svg" />
      <label>Check me</label>
    </div>
  </div>
```

<blockquote>
    <sub>
    	<strong>Note</strong>: class `svg` to be added in img tag or svg tag.
    </sub>
</blockquote>

<div align="right">
 <i><sub><a href="https://lokesh-coder.github.io/pretty-checkbox#svg">more details</a></sub></i>
</div>

<div align="center"><strong >---</strong></div>

#### Image

Supports any type of valid image format.

```html
  <div class="pretty p-image">
    <input type="checkbox" />
    <div class="state">
      <img class="image" src="/check.png" />
      <label>Block</label>
    </div>
  </div>
```

<blockquote>
    <sub>
    	<strong>Note</strong>: class `image` to be added in img tag.
    </sub>
</blockquote>

<div align="right">
 <i><sub><a href="https://lokesh-coder.github.io/pretty-checkbox#image">more details</a></sub></i>
</div>

<div align="center"><strong >---</strong></div>

#### Colors

There are five solid colors `p-primary` `p-success` `p-warning` `p-info` `p-danger`

And five outline colors  `p-primary-o` `p-success-o` `p-warning-o` `p-info-o` `p-danger-o`

```html
  <div class="pretty p-default p-curve p-thick">
    <input type="checkbox" />
    <div class="state p-warning">
      <label>Warning</label>
    </div>
  </div>
```
<blockquote>
    <sub>
    	<strong>Note</strong>: Color class must be added in state class. Solid colors and Ouline colors have distinct role in font icons and toggle feature.
    </sub>
</blockquote>

<div align="right">
 <i><sub><a href="https://lokesh-coder.github.io/pretty-checkbox#colors">more details</a></sub></i>
</div>

### More

There are more features like  ***Radio buttons*** , ***Toggle*** , ***States*** , ***Animations*** , ***Border less*** , ***Lock*** , ***Scale***, ***SCSS Settings***. 

Please refer the [documentation](https://lokesh-coder.github.io/pretty-checkbox/) to know about them.


### Browser support

Works in all modern browsers.

`Chrome >= 26` `Firefox >= 16` `Safari >= 6.1` `Opera >= 15` `IE >= 9`

### Font Icon libraries
* [Font awesome](http://fontawesome.io/icons/)
* [Bootstrap Glyphicons](https://getbootstrap.com/docs/3.3/components/#glyphicons)
* [Material icon ( MDI )](https://materialdesignicons.com/)
* [Material icon ( ZMDI )](http://zavoloklom.github.io/material-design-iconic-font/icons.html)
* [Ion icons](http://ionicons.com/)
* [Typicons](http://www.typicons.com/)
* [Material icon ( Google )](https://material.io/icons)
* Others not tested, but will work ( 99% ).


### SVG
* [UIKit](https://getuikit.com/docs/icon)
* [Feathers](https://feathericons.com/)
* Others

### Libraries
- VueJs - [pretty-checkbox-vue](https://github.com/hamed-ehtesham/pretty-checkbox-vue)
- Angular - [ngx-pretty-checkbox](https://github.com/miladfm/ngx-pretty-checkbox)

### Inspiration
- [Awesome Bootstrap Checkbox](https://github.com/flatlogic/awesome-bootstrap-checkbox) - Idea
- [Animista](http://animista.net) - Animations

### Contributions
Thanks to all those good people who spend their valuable time and helped to improve this library. Any Contributions are welcome!

### License
This project is licensed under the MIT License


<div align="center"><sub>❤</sub></div> 

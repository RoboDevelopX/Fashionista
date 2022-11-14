# Fashionista

*This repo is solely developed for the purpose of Final-Year-Project by CSE & IT students, GGI.*

(*For use of educational purposes only. This repo will no longer be maintained after project submission.*)



## Contents

- [Getting Started](#getting-started)
- [Switch CSS Layouts](#switch-css-layouts)
- [Change Features](#change-features)
- [Sources and Credits](#sources-and-credits)




## Getting Started

Fashionista is a new, clean and polish multipurpose - commerce website built with modern workflow. When developing this website, we highly focused on some goals i.e., responsiveness, well tested on all compatible browsers designed to be reusable and could be easily customizable into any stores like clothing, toys, mobiles & tablets, electronics, books, furniture etc.
Fashionista is Front-end for an e-commerce clothes selling website.


## Switch CSS Layouts

Inside the **css** folder we have all the stylesheets and vendor dependencies which our layout needs. You can use the color scheme according to your likeness.

- css/bundle.css **(Default color scheme)**
- css/bundle.black.css **(black color scheme)**
- css/bundle.blue.css **(blue color scheme)**
- css/bundle.green.css **(green color scheme)**
- css/bundle.green-munsell.css **(green-munsell color scheme)**
- css/bundle.orange.css **(orange color scheme)**
- css/bundle.pink.css **(pink color scheme)**
- css/bundle.purple.css **(purple color scheme)**
- css/bundle.skyblue.css **(skyblue color scheme)**



## Change Features

**1. Disable Modal**

Default when you visit the **Homepage** a newsletter modal will pop up. You can disable the newsletter modal by editing the file `app.js`. This file has 6 different sections, every section starts with the comment. So this is on the **Homepage** function which is called section no 3.

```javascript
/*============================================================================*/
/* Homepage JavaScript functions
/*============================================================================*/
$(function () {
    showNewsletterModal();
     // showNewsletterModal(); Comment this function
});
```

Comment this function then newsletter modal will not show.

**2. Slider Options**

All sliders invocation are **Homepage JavaScript functions** which are also section no 3 on `app.js` file. You can modify the slider options by editing the file.

```javascript
/*============================================================================*/
/* Homepage JavaScript functions
/*============================================================================*/
/**
 * Initialize Main Slider
 */
const sliderMain = function() {
    let $owl = $('.slider-main');
	$owl.owlCarousel({});
};
/**
 * Initialize owl-carousel for all product-place section on page
 */
const productSlider = function() {};
/**
 * Initialize owl-carousel for all Specific Category section on page
 */
const SpecificCategorySlider = function() {};
/**
 * Initialize owl-carousel for brand slider
 */
const brandSlider = function() {};
```

**3. Disable Countdown**

**Homepage** has a countdown section. You can disable the countdown from the section, just erase the class `dynamic` from the div.

```html
<div class="section-timing-wrapper dynamic">
```

**4. Disable Backdrop**

Default when you focus on **mega drop downs** and **search input** you will see on **html** pages some **backdrop effect** will appear, to disable this **effect** you can edit the file `app.js`. It's on section no 2 which is also called **Global JavaScript functions**.

```javascript
/*============================================================================*/
/* Global JavaScript functions
/*============================================================================*/

// Object Settings

let settings = {
     bodyBackDropOnScenes: true, // Change this property to false 'bodyBackDropOnScenes: false'
    zIndexNumber: 999998
    };
```

**4. Change color scheme**

All **.html** pages are included with default color scheme i.e. `bundle.css`.

```html
<!DOCTYPE html>
<html class="no-js" lang="en-US">

<head>
    <meta charset="UTF-8">
    <!--[if IE]>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <![endif]-->
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
    <meta name="description" content="">
    <meta name="author" content="">
    <title>Groover - Online Shopping for Electronics, Apparel, Computers, Books, DVDs & more</title>
    <!-- Standard Favicon -->
    <link href="favicon.ico" rel="shortcut icon">
    <!-- Base Google Font for Web-app -->
    <link href="https://fonts.googleapis.com/css?family=Open+Sans:400,700" rel="stylesheet">
    <!-- Google Fonts for Banners only -->
    <link href="https://fonts.googleapis.com/css?family=Raleway:400,800" rel="stylesheet">
    <!-- Vendor -->
    <link rel="stylesheet" href="css/vendor.css">
    <!-- Utility -->
    <link rel="stylesheet" href="css/utility.css">
    <!-- Main -->
    <link rel="stylesheet" href="css/bundle.css"> <!--- Default color scheme -->
```

You can change the stylesheet according to your **color scheme**, just erase the old `<link>` tag with the new one.

```html
<link rel="stylesheet" href="css/bundle.blue.css">
```

**5. Change Tab on a Section**

You can see **tabs** in all sections. Default we have made 2 tabs for a section.

- Horizontal Tab:
- Vertical Tab:

Every **tab** has 4 different styles which is written on `_section-maker.scss` file. You can change the style.

In **home.html** file for **horizontal-tabs** you can use these classes.

```html
<ul class="nav tab-nav-style-1-a justify-content-center">

<!-- You can erase the old class and add a new class -->

<ul class="nav tab-nav-style-1-b justify-content-center">

<ul class="nav tab-nav-style-1-c justify-content-center">

<ul class="nav tab-nav-style-1-d justify-content-center">
```

For **vertical-tabs** you can use these classes.

```html
<ul class="nav tab-nav-style-2-a justify-content-center">

<!-- You can erase the old class and add a new class -->

<ul class="nav tab-nav-style-2-b justify-content-center">

<ul class="nav tab-nav-style-2-c justify-content-center">

<ul class="nav tab-nav-style-2-d justify-content-center">
```

**6. Change Banner Hover Effect**

Default all banners on layout have **opacity effect**, which is shown when you hovering on banners. All hover effects are written on **src/scss/components/_banners-hover-effect.scss** file. You can change this.

```html
<a href="shop-v1-root-category.html" class="mx-auto banner-hover effect-dark-opacity">

<!-- Erase the effect- class, and add the new one -->

<a href="shop-v1-root-category.html" class="mx-auto banner-hover effect-border-scaling-gray">

<a href="shop-v1-root-category.html" class="mx-auto banner-hover effect-border-scaling-black">
```

**7. Change Page Breadcrumb background**

When you open some **html** pages you will see those pages have background picture on the breadcrumb. You can also change this, all variations are written on **src/scss/base/_pre-config.scss** file.

```html
<!-- Page Introduction Wrapper -->

<div class="page-style-a">

<!-- Erase the old class, add the new one -->

<div class="page-style-b">

<div class="page-style-c">
```



## Sources and Credits

- [Node.JS - JavaScript Environment](https://nodejs.org/en/download/)
- [Bootstrap 4](https://getbootstrap.com/)
- [jQuery](https://jquery.com/)
- [jQuery UI Range Slider](https://jqueryui.com/slider/)
- [Font Awesome 5](https://fontawesome.com/)
- [Ion Icons 4](https://ionicons.com/)
- [Owl Carousel 2](https://owlcarousel2.github.io/OwlCarousel2/)
- [Animate.css](https://daneden.github.io/animate.css/)

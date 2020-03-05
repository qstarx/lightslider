![license](https://img.shields.io/npm/l/lightslider.svg)
![travis](https://travis-ci.org/sachinchoolur/lightslider.svg?branch=master)
![bower](https://img.shields.io/bower/v/lightslider.svg)
![npm](https://img.shields.io/npm/v/lightslider.svg)

jQuery lightSlider
=============

This is a fork from https://github.com/sachinchoolur/lightslider

Description
===========

** This Version adds automatic generation of thumbs for pager **

- First Method uses [html2canvas](https://github.com/niklasvh/html2canvas). 

      canvas: true
      canvasScale: 0.5
    
- Second method clones the HTML markup and applies a custom style

      clonePager: true,
      pagerClass: "my-custom-class",

** Another functionallity is a possible callback function for paging **

Its possible to create a second pager and set an active class through the callback:

      pagerCallback: function (act) { 
        $('.mypager a').removeClass('active')
        $('.mypager a:nth-child('+(act+1)+')').addClass('active')
      }

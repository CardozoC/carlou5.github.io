---
layout: post
title: Responsive Layouts intimidating you? Not anymore.
---
<link href="//maxcdn.bootstrapcdn.com/bootstrap/3.3.4/css/bootstrap.min.css" rel="stylesheet">


Often, we Web Designers hear that our sites should be mobile-friendly or responsive... It can be hard to choose how to make a responsive site with so many options available to achieve this. The next best thing is always changing, so it is a bit intimidating to dive into a new programming language or framework. 

There is one CSS Framework that can help you with this mess: Bootstrap. By linking Bootstrap to your site, you can simply add classes to your tags in order to style them. The combination of some classes and your div tags will make your reponsive layouts a breeze to create. So to help you expand into responsive layouts, I'll show you a few tricks to incorporate Bootstrap easily into your site.

##Bootstrap 101

###1. Link the bootstrap file to your website

There are two ways to link the boostrap css file to your site. 

You can download the boostrap css file and host it on your server
`<link href="/yourfolder/bootstrap.css" rel="stylesheet">`

Or, you can link directly to a CDN (content delivery network) like the one below. This is the better option because it faster and will likely be cached in your browser from another site that also used it.
`<link href="//maxcdn.bootstrapcdn.com/bootstrap/3.3.4/css/bootstrap.min.css" rel="stylesheet">`

###2. Learn the Bootstrap Basics

Grid systems are used for creating page layouts through a series of rows and columns that house your content. Here's how the Bootstrap grid system works:

-Rows must be placed within a .container (fixed-width) or .container-fluid (full-width) for proper alignment and padding.
-Use rows to create horizontal groups of columns.
-Content should be placed within columns, and only columns may be immediate children of rows.
-Predefined grid classes like .row and .col-xs-4 are available for quickly making grid layouts. Less mixins can also be used for more semantic layouts.
-Columns create gutters (gaps between column content) via padding. That padding is offset in rows for the first and last column via negative margin on .rows.
-The negative margin is why the examples below are outdented. It's so that content within grid columns is lined up with non-grid content.
-Grid columns are created by specifying the number of twelve available columns you wish to span. For example, three equal columns would use three .col-xs-4.
-If more than 12 columns are placed within a single row, each group of extra columns will, as one unit, wrap onto a new line.
-Grid classes apply to devices with screen widths greater than or equal to the breakpoint sizes, and override grid classes targeted at smaller devices. Therefore, e.g. applying any .col-md-* class to an element will not only affect its styling on medium devices but also on large devices if a .col-lg-* class is not present.

###3. Example

<div class="row">
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
</div>
<div class="row">
  <div class="col-md-8">.col-md-8</div>
  <div class="col-md-4">.col-md-4</div>
</div>
<div class="row">
  <div class="col-md-4">.col-md-4</div>
  <div class="col-md-4">.col-md-4</div>
  <div class="col-md-4">.col-md-4</div>
</div>
<div class="row">
  <div class="col-md-6">.col-md-6</div>
  <div class="col-md-6">.col-md-6</div>
</div>

The layout above is created with this code:
`<div class="row">
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
  <div class="col-md-1">.col-md-1</div>
</div>
<div class="row">
  <div class="col-md-8">.col-md-8</div>
  <div class="col-md-4">.col-md-4</div>
</div>
<div class="row">
  <div class="col-md-4">.col-md-4</div>
  <div class="col-md-4">.col-md-4</div>
  <div class="col-md-4">.col-md-4</div>
</div>
<div class="row">
  <div class="col-md-6">.col-md-6</div>
  <div class="col-md-6">.col-md-6</div>
</div>
</code>`

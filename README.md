#jQuery Wrapper for [PhotoSwipe](https://github.com/dimsemenov/photoswipe)

This plugin will allow you to easily transition from your existing fancybox/lightbox plugins to PhotoSwipe without altering you HTML layout or finding a way define image dimensions. Plugin gets your existing html layout and creates all structure needed for [PhotoSwipe](https://github.com/dimsemenov/photoswipe).

##Usage

Here I used fancybox class but it's up to you to change it.

###Includes
    <!-- jQuery -->
    <script src="path/to/jquery.min.js"></script> 

    <!-- PhotoSwipe Core CSS file -->
    <link rel="stylesheet" href="path/to/photoswipe.css"> 

    <!-- PhotoSwipe Skin CSS file (styling of UI - buttons, caption, etc.)
    <link rel="stylesheet" href="path/to/default-skin/default-skin.css"> 

    <!-- PhotoSwipe Core JS file -->
    <script src="path/to/photoswipe.min.js"></script> 

    <!-- PhotoSwipe UI JS file -->
    <script src="path/to/photoswipe-ui-default.min.js"></script>

    <!-- esPhotoSwipe JS file -->
    <script src="path/to/esPhotoSwipe.min.js"></script> 

###HTML

**Single Image**

    <a class="fancybox" href="http://lorempixel.com/1024/768/" title="Photo Caption #1" alt="Photo Caption #1"><img src="http://lorempixel.com/320/200/" border="0"></a>

**Image Gallery**

    <a class="fancybox" href="http://lorempixel.com/1024/768/" data-fancybox-group="uniquegalleryname" title="Photo Caption #1" alt="Photo Caption #1"><img src="http://lorempixel.com/320/200/" border="0"></a>
    <a class="fancybox" href="http://lorempixel.com/1024/768/" data-fancybox-group="uniquegalleryname" title="Photo Caption #2" alt="Photo Caption #2"><img src="http://lorempixel.com/320/200/" border="0"></a>
    <a class="fancybox" href="http://lorempixel.com/1024/768/" data-fancybox-group="uniquegalleryname" title="Photo Caption #3" alt="Photo Caption #3"><img src="http://lorempixel.com/320/200/" border="0"></a>

###JavaScript

    $(document).ready(function () {
        $(".fancybox").esPhotoSwipe();
    });

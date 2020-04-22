# custom_fancybox
***Using this plugin, you can display an enlarged image in a separate window when you click on a thumbnail, organize a gallery of slides with navigation and simply display a pop-up window.***


# Create a photo gallery.

First you need to download the ***custom_fancybox.js*** and ***styles.css*** files.

Now write simple HTML for photo gallery:

``` html
<div class="container ">
        <div class="common_div" >
            <a href="#" class="photo">
                <img src="../code/img/1.jpg" alt="" class="eachPhoto" >
            </a>
            <a href="#" class="photo">
                <img src="../code/img/2.jpg" alt="" class="eachPhoto">
            </a>
            <a href="#" class="photo" >
                <img src="../code/img/3.jpg" alt="" class="eachPhoto">
            </a>
            <a href="#" class="photo" >
                <img src="../code/img/6.jpg" alt="" class="eachPhoto">
            </a>
       </div>
</div>
```
Connect JavaScript:

```html
<script src="../code/js/custom_fancybox.js"></script>
```

Also you need to add this in your HTML:

```html
<link rel="stylesheet" href="../code/css/styles.css">
```

To use, you must call the method __*fancybox()*__ in your file JavaScript. For example:

```js
let container_box = document.querySelector('.container')
container_box.fancybox({
    margin: 10,
});
```

You can set the distance between photos using the margin parameter or use the default parameter.

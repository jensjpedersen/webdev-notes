


# Hide image overflow
* Set `overflow: hidden` in image container (parent element)

```css
.image-container {
    width: 500px; 
    height: 500px;
    overflow: hidden; 
}

img {
    width: 200%;
    height: auto;
}
```

# Image Properties
* `opacity` - 0 to 1
* `filter` - blur, brightness, contrast, drop-shadow, grayscale, hue-rotate, invert, opacity, saturate, sepia

* `object-fit` - how the image should fill its container. Changes aspect ratio of image
    * fill (default) - The image will be stretched or squished to fit the
      container, dependent on width and height
    * contain - The image keeps its aspect ratio, but is resized to fit within the given dimension
    * cover ( **Best** ) - The image keeps its aspect ratio and fills the given dimension. The image will be clipped to fit
    * none - The image is not resized
    * scale-down - the image is scaled down to the smallest version of none or contain


## Convert parent container 
* This will not overflow the container, due to width and height being 100% of the parent container
* will overflow the container if width and/or height is greater than 100% of the parent container
* Parts of image may be cut off, due to aspect ratio of image not matching the aspect ratio of the container
```css
img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}
```




# Image Hover Overlay
* Create an overlay effect on hover: [CSS Styling Images](https://www.w3schools.com/css/css3_images.asp)


# Adjusting image position
## Center image with flex
```css
display: flex; 
justify-content: center; 
align-items: center; 
```

## Position image with absolute
* Need to set parent container to `position: relative`. 
This will allow the child element to be positioned relative to the parent element
* Else, the child element will be positioned relative to the entire page

```css
.img_container {
    position: relative;
}

img {
position: absolute;
top: 50%;
left: 50%;
transform: translate(-50%, -50%);
}
```




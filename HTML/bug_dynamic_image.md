

* This is my html code: 
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title></title>
        <link rel="stylesheet" href="style.css">
    </head>
    <body>


        <div class="gallery">

            <div class="image-container"> <img src="Images/bg_13.jpg"> </div>
            <div class="image-container"> <img src="Images/bg_15.jpg"> </div>
            <div class="image-container"> <img src="Images/bg_16.jpg"> </div>
            <div class="image-container"> <img src="Images/bg_17.jpg"> </div>
            <div class="image-container"> <img src="Images/bg_18.jpg"> </div>
            <div class="image-container"> <img src="Images/bg_19.jpg"> </div>
            <div class="image-container"> <img src="Images/bg_20.jpg"> </div>
            <div class="image-container"> <img src="Images/bg_23.jpg"> </div>
            <div class="image-container"> <img src="Images/bg_27.jpg"> </div>
            <div class="image-container"> <img src="Images/bg_29.jpg"> </div>
            <div class="image-container"> <img src="Images/bg_2.jpg"> </div>
            <div class="image-container"> <img src="Images/bg_3.jpg"> </div>
            <div class="image-container"> <img src="Images/bg_4.jpg"> </div>
            <div class="image-container"> <img src="Images/bg_5.jpg"> </div>
            <div class="image-container"> <img src="Images/bg_7.jpg"> </div>


        </div>



    </body>
</html>
```

This is my css code: 
```css


div.image-container {
    width: 100vw;
    height: auto; 
}

img {
    height: 100%; 
    width: 100%
} 

```

The images shoudl dynamicly reszie dependent on the view width, but this only
works down to a width of 245px, why?

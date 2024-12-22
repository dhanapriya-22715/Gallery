# Date:22-11-2024
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
html
<!DOCTYPE html>
<html>
<head>
    <meta name="viewport" content="width=device-width , initial-scale=1.0">
    <title>Image Gallery</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="full-img" id="fullImgBox">
        <img src="img gallery-1.jpg" id="fullImg">
        <span onclick="closeFullImg()">X</span>
    </div>

    <div class="img-gallery">
        <img src="img gallery-1.jpg" onclick="openFullImg(this.src)">
        <img src="img gallery-2.jpg" onclick="openFullImg(this.src)">
        <img src="img gallery-3.jpg" onclick="openFullImg(this.src)">
        <img src="img gallery-4.jpg" onclick="openFullImg(this.src)">
        <img src="img gallery-5.jpg" onclick="openFullImg(this.src)">
        <img src="img gallery-6.jpg" onclick="openFullImg(this.src)">
        <img src="img gallery-7.jpg" onclick="openFullImg(this.src)">
        <img src="img gallery-8.jpg" onclick="openFullImg(this.src)">
        <img src="img gallery-9.jpg" onclick="openFullImg(this.src)">
    </div>

<script>
    var fullImgBox = document.getElementById("fullImgBox");
    var fullImg = document.getElementById("fullImg");

    function openFullImg(pic){
        fullImgBox.style.display="flex";
        fullImg.src = pic;
    }

    function closeFullImg(){
        fullImgBox.style.display="none";

    }
</script>
</body>
</html>

css 
*{
    margin: 0;
    padding: 0;
    font-family:sans-serif;
}
body{
    background: #ecf4fb;
}
.img-gallery{
    width: 70%;
    margin: 100px auto 50px;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px,1fr));
    grid-gap:30px;
}
.img-gallery img{
    width: 100%;
    height: 100%;
    cursor:pointer;
}
.img-gallery img:hover{
    transform: scale(0.8) rotate(-25deg);
    border-radius: 20px;
    box-shadow: 0 32px 75px rgba(68,77,136,0.2);

}
.full-img{
    width: 100%;
    height: 100vh;
    background: rgba(0,0,0,0.9);
    position: fixed;
    top: 0;
    left: 0;
    display: none;
    align-items: center;
    justify-content: center;
    z-index: 100;

}
.full-img img{
    width: 90%;
    max-width: 500px;
}
.full-img span{
    position: absolute;
    top: 5%;
    right: 5%;
    font-size: 30px;
    color: #fff;
    cursor:pointer;

}
```


# OUTPUT:
![Screenshot (60)](https://github.com/user-attachments/assets/6b1054ea-c386-4bd3-afdc-d2eb00ddb306)
![Screenshot (61)](https://github.com/user-attachments/assets/2ffde2c1-416d-400c-ad00-079d4ac49333)
![Screenshot (62)](https://github.com/user-attachments/assets/13d17c96-9a9d-4c5f-a9f6-85dd8c6762c9)
![Screenshot (63)](https://github.com/user-attachments/assets/40936cd3-1b13-46b1-9c89-dd165095083a)
![Screenshot (64)](https://github.com/user-attachments/assets/4a5f965e-396c-4e7d-8097-dbed9c13f06b)
![Screenshot (65)](https://github.com/user-attachments/assets/4f672529-dbe3-46ff-a33a-96d9000c37fc)
![Screenshot (66)](https://github.com/user-attachments/assets/72397256-3bb0-4bcf-b6aa-12d3796a3376)
![Screenshot (67)](https://github.com/user-attachments/assets/fa295a87-888f-413d-abc2-94ffb302b6ec)
![Screenshot (68)](https://github.com/user-attachments/assets/8dbc3d13-756f-485f-8967-eb8cffe16e5d)
![Screenshot (69)](https://github.com/user-attachments/assets/71e285be-b100-4949-84c0-e039ecebc11d)



# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.

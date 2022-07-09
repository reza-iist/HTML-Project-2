![cover](./cover.png)  
# HTML-Project-2
Create a Web Design using HTML &amp; CSS Project-2  
---
### Youtube Link of HTML-Project-2  
[Web Design-Project-2](https://youtu.be/aqvRafv_5nc)  
---
### Playlists Links for Web Design, Web Development of me  
1. [Web-Design-Project-1](https://www.youtube.com/playlist?list=PLxqLmn_MNa-Sl7EtwOFCV4zWEwleEd3mk)  
2. [Web-Design-Project-2](https://www.youtube.com/playlist?list=PLxqLmn_MNa-Rfie-DoTgRRnUnXxZKGZip)  
3. [Web-Development-Level-IV Certificate](https://www.youtube.com/playlist?list=PLxqLmn_MNa-Sv8NyBi2i97qDElbCeWcdW)
---
### HTML Code  
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML-Project-2</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Header Part Start -->
    <header>
        <nav class="navbar">
            <img src="./assets/images/cropped-iist-logo-2.png" alt="iist-logo" class="logo">
            <h1>IIST</h1>
            <ul class="nav-list">
                <li class="list-item"><a href="#">Home</a></li>
                <li class="list-item"><a href="#">About Us</a></li>
                <li class="list-item"><a href="#">Courses</a></li>
                <li class="list-item"><a href="#">Admission</a></li>
                <li class="list-item"><a href="#">Contact</a></li>
            </ul>
        </nav>
        <div class="header-cont">
            <h1>Ideal Institute of Science & Technology</h1>
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit.<br> Inventore quaerat nemo, earum<br> nobis quos sed illo a fugit incidunt perferendis!</p>
            <a href="#" class="learn-more">Learn More</a>
            <a href="https://iist-mirpur.edu.bd/online-application/" target="_blank" class="btn">Apply Now</a>
        </div>
    </header>
    <!-- Header Part End -->
</body>
</html>
~~~  

### Style.css code  

~~~
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
/* common css end*/
/* Header part start*/
body{
    font-family: roboto,sans-serif;
}
body h1, body h2{
    color: #ccccff;
}
body p{
    color: #9c9c9c;
}
header{
    width: 1200px;
    min-height: 90vh;
    margin: 0 auto;
    background:linear-gradient(rgba(0,0,0,0.8),rgba(0,0,0,0.8)), url(./assets/images/electrical-lab-5.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center center;
}
.navbar{
    width: 100%;
    height: 100px;
    display: flex;
    padding: 0 20px;
    align-items: center;
}
.navbar h1{
    padding-left: 20px;
    font-size: 40px;
}
.logo{
    width: 50px;
    height: 50px;
}
.nav-list{
    list-style: none;
    display: flex;
    padding-left: 600px;
}
.list-item a{
    text-decoration: none;
    padding-left: 20px;
    color: whitesmoke;
    font-size: 16px;
}
.list-item a:hover{
    color: aqua;
}
.list-item{
    position: relative;
}
.list-item::after{
    content: " ";
    position: absolute;
    width: 0%;
    height: 2px;
    background: aqua;
    left: 20px;
    bottom: -5px;
    transition: 0.5s;
}
.list-item:hover::after{
    width: 75%;
}
.header-cont{
    position: absolute;
    top: 50%;
    width: 90%;
    text-align: center;
    transform: translateY(-50%);
}
.header-cont h1{
    font-size: 40px;
}
.header-cont p{
    padding: 20px 0;
}
.header-cont a{
    padding: 5px 30px;
    text-decoration: none;
    font-size: 20px;
    color: tomato;
    border:2px solid aqua;
    border-radius: 20px;
    margin-right: 20px;
    position: relative;
    
}
.header-cont a::after{
    content: " ";
    position: absolute;
    width: 0%;
    height: 100%;
    background: green;
    left: 0;
    top: 0;
    z-index: -1;
    border-radius: 20px;
    transition:0.5s;
}
.header-cont a:hover::after{
    width: 100%;
}
/* Header part end*/
~~~

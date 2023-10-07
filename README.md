<!DOCTYPE html>
<!-- Coding By CodingNepal - www.codingnepalweb.com -->
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"/>
    <title>Coffee Website HTML and CSS | CodingNepal</title>
    <link rel="stylesheet" href="style.css">
    <!-- Google Fonts Links For Icon -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css" />
    <style>
      /* Importing Google font - Poppins */
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}
body{
  
  align-items: center;
  justify-content: center;
}

header {
position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  padding: 20px;
}

header .navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
}

.navbar .logo {
  color: #fff;
  font-weight: 600;
  font-size: 2.1rem;
  text-decoration: none;
}

.navbar .logo span {
  color: #C06B3E;
}

.navbar .menu-links {
  display: flex;
  list-style: none;
  gap: 35px;
}

.navbar a {
    font-size: 1.3rem;
  color: #fff;
  text-decoration: none;
  transition: 0.2s ease;
}

.navbar a:hover {
  color: #C06B3E;
}

.hero-section {
  height: 100vh;
  background-image: url("black-car.jpg");
  background-position: center;
  background-size: cover;
  display: flex;
  align-items: center;
  padding: 0 20px;
}

.hero-section .content-1 {
  max-width: 1200px;
  margin: 0 auto;
  width: 100%;
  color: #fff;
}

.hero-section .content-1 h2 {
  font-size: 3rem;
  max-width: 600px;
  line-height: 70px;
}

.hero-section .content-1 p {
    font-size: 25px;
  font-weight: 300;
  max-width: 600px;
  margin-top: 15px;
}

.hero-section .content-1 button {
  width: 50%;
  background:#fff;
  border-color: #fff;
  padding: 12px 30px;
  border: none;
  font-size: 1rem;
  border-radius: 20px;
  margin-top: 38px;
  cursor: pointer;
  font-weight: 500;
  transition: 0.2s ease;
}

.hero-section .content-1 button:hover {
  color: #fff;
  background: #C06B3E;
  scale: 1.1;
}

#close-menu-btn {
  position: absolute;
  right: 20px;
  top: 20px;
  cursor: pointer;
  display: none;
}

#hamburger-btn {
  color: #fff;
  cursor: pointer;
  display: none;
}

@media (max-width: 768px) {
  header {
    padding: 10px;
  }

  header.show-mobile-menu::before {
    content: "";
    position: fixed;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    backdrop-filter: blur(5px);
  }

  .navbar .logo {
    font-size: 1.7rem;
  }

    
  #hamburger-btn, #close-menu-btn {
    display: block;
  }

  .navbar .menu-links {
    position: fixed;
    top: 0;
    left: -250px;
    width: 250px;
    height: 100vh;
    background: #fff;
    flex-direction: column;
    padding: 70px 40px 0;
    transition: left 0.2s ease;
  }

  header.show-mobile-menu .navbar .menu-links {
    left: 0;
  }

  .navbar a {
    color: #000;
  }

  .hero-section .content {
    text-align: center;
  }

  .hero-section .content :is(h2, p) {
    max-width: 100%;
  }

  .hero-section .content h2 {
    font-size: 2.3rem;
    line-height: 60px;
  }
  
  .hero-section .content button {
    padding: 9px 18px;
  }
}
.scrollable-area {
    width: 1902px; /* Kaydırılabilir alanın genişliği */
    height: 1000px; /* Kaydırılabilir alanın yüksekliği */
    overflow: auto; /* İçeriği aşan kısmı kaydırılabilir yapın */
    background-color: black;
    background-image: url("wp7605371.png");
    background-position: center;
    background-size: cover;
    display: flex;
    align-items: center;
    padding: 0 20px;
  }

  .contact{
    background:url(bg5.jpg);
    height: 980px;
    background-repeat: no-repeat;
    background-position:fixed;
    background-size: cover;
  }
 

  

.wrapper{
  margin-top:20vh; ;
  float:right;
  margin-right: 300px;
  display: flex;
  max-width: 1200px;
  position: relative;
}
.wrapper i{
  top: 50%;
  height: 44px;
  width: 44px;
  color: #343F4F;
  cursor: pointer;
  font-size: 1.15rem;
  position: absolute;
  text-align: center;
  line-height: 44px;
  background: #fff;
  border-radius: 50%;
  transform: translateY(-50%);
  transition: transform 0.1s linear;
}
.wrapper i:active{
  transform: translateY(-50%) scale(0.9);
}
.wrapper i:hover{
  background: #f2f2f2;
}
.wrapper i:first-child{
  left: -22px;
  display: none;
}
.wrapper i:last-child{
  right: -22px;
}
.wrapper .carousel{
  font-size: 0px;
  cursor: pointer;
  overflow: hidden;
  white-space: nowrap;
  scroll-behavior: smooth;
}
.carousel.dragging{
  cursor: grab;
  scroll-behavior: auto;
}
.carousel.dragging img{
  pointer-events: none;
}
.carousel img{
 transition: filter 0.3s ease;
  height: 340px;
  object-fit: cover;
  user-select: none;
  margin-left: 14px;
  width: calc(100% / 3);
}
.carousel img:first-child{
  margin-left: 0px;
}
@media screen and (max-width: 900px) {
  .carousel img{
    width: calc(100% / 2);
  }
}
@media screen and (max-width: 550px) {

  .carousel img{
    width: 100%;
  }
}
@media screen and (max-width:425px) {
    .wrapper{
       margin-right: 0px;
       margin-top: 40vh;
    }
    .carousel img{
        width: 100%;
    }
    .carousel{
        margin:0px;
    }
    #left{
        margin-left: -15px;
    }
    #right{
        margin-right:20px
    }
}

#image:hover {
    filter: brightness(0.8); /* Hover'da parlaklığı azaltın */
}
.table{
    padding: 20px 20px 20px 20px;
    border-radius: 10px;
}
.table h1{
  color:cadetblue;
 font-size: 40px;
    width: 100%;
    font-family: 'Poppins', sans-serif;
   
}
.call-ph{
  background:#C06B3E;
  height: 980px;
  background-repeat: no-repeat;
  background-position:fixed;
  background-size: cover;
}

.cards{
  max-width: 1100px;
  margin: 0 auto;
  text-align: center;
  padding: 30px;
}
.cards h2.header{
  font-size: 40px;
  margin: 0 0 30px 0;
  text-transform: uppercase;
  letter-spacing: 1px;
}
.services2{
  margin-top: 200px;
  display: flex;
  align-items: center;
}
.content{
  display: flex;
  flex-wrap: wrap;
  flex: 1;
  margin: 20px;
  padding: 20px;
  border: 2px solid black;
  border-radius: 4px;
  transition: all .3s ease;
}
.content .fab{
  font-size: 70px;
  margin: 16px 0;
}
.content > *{
  flex: 1 1 100%;
}
.content:hover{
  color: white;
}
.content:hover a and #copyButton{
  border-color: white;
  background: white;
  color: #000;
}

.content h2{
  font-size: 30px;
  margin: 16px 0;
  letter-spacing: 1px;
  text-transform: uppercase;
}
.content p{
  font-size: 17px;
  font-family: 'Poppins',sans-serif;
}
.content a{
  margin: 22px 0;
  background: black;
  color: white;
  text-decoration: none;
  text-transform: uppercase;
  border: 1px solid black;
  padding: 15px 0;
  border-radius: 25px;
  transition: .3s ease;
}
.content a:hover{
  border-radius: 10px;
}
@media (max-width: 900px) {
  .services{
    display: flex;
    flex-direction: column;
  }
}
#btn-i{
  font-size: 70px;
}
#copyButton{
  margin: 22px 0;
  background: black;
  color: white;
  text-decoration: none;
  text-transform: uppercase;
  border: 1px solid black;
  padding: 15px 0;
  border-radius: 25px;
  transition: .3s ease;
}
#copyButton:hover{
  border-radius: 10px;
}
.rating{
  display: grid;
  height: 100%;
  place-items: center;
  text-align: center;
  background: #000;
  height: 980px;
  background-repeat: no-repeat;
  background-position:fixed;
  background-size: cover;
}


    </style>
  </head>
  <body>
    <header>
      <nav class="navbar">
        <a class="logo" href="#" >Ces-Travel</Cest-Travel><span>.</span></a>
        <ul class="menu-links">
          <span id="close-menu-btn" class="material-symbols-outlined">close</span>
          <li><a onclick="refreshPage()">Ana Menü</menu></a></li>
          <li><a href="#">Bize ulaş</a></li>
          <li><a href="#">Hesaplar</a></li>
          <li><a href="#">Hakkımızda</a></li>
        </ul>
        <span id="hamburger-btn" class="material-symbols-outlined">menu</span>
      </nav>
    </header>

    <section class="hero-section">
      <div class="content-1">
        <h2>Seyahat,Her yerde Seyahat</h2>
        <p>
            “Dünyayı dolaşın. Görebileceğiniz bütün rüyaların en muhteşemi!” – Ray Bradbury
        </p>
       <a href="#services"> <button onclick="goToPage('page2')" href="#services">Turlarımız</button> </a>
      </div>
    </section>

    <section class="contact" id="services"> 
        
        <div class="wrapper" id="image">
            <div class="table">
                <h1>Turlarımız...</h3>
            <i id="left" class="fa-solid fa-angle-left"></i>
            <div class="carousel">
              <img src="bursa3.jpg" alt="img" draggable="false">
              <img src="bursa1.jpg" alt="img" draggable="false">
              <img src="bursa-ulu-cami.jpg" alt="img" draggable="false">
              <img src="WhatsApp Image 2023-10-07 at 11.10.36.jpeg" alt="img" draggable="false">
              <img src="WhatsApp Image 2023-10-07 at 11.10.35 (1).jpeg" alt="img" draggable="false">
              <img src="WhatsApp Image 2023-10-07 at 11.10.35.jpeg" alt="img" draggable="false">
              <img src="WhatsApp Image 2023-10-07 at 11.14.11 (2).jpeg" alt="img" draggable="false">
              <img src="WhatsApp Image 2023-10-07 at 11.14.11 (1).jpeg" alt="img" draggable="false">
              <img src="WhatsApp Image 2023-10-07 at 11.14.11.jpeg" alt="img" draggable="false">
            
            </div>
            <i id="right" class="fa-solid fa-angle-right"></i>
            
           
          </div>

        </div>
      


    </section>

    <section class="call-ph">
      <div class="phone">
        <div class="cards">
          <h2 class="header">
            
          </h2>
          <div class="services2">
             <div class="content content-1">
                <div  class="fab fa-instagram"></div>
                <h2>
                   İnstagram
                </h2>
                <p>
                   İnstagram Adresimize erişmek için tıkla!
                </p>
                <a href="https://www.instagram.com/ces_travel_vip_transfer/?igshid=MWZjMTM2ODFkZg%3D%3D">Ces-Travel</a>
                <h3>Telefondan Ulaşmak İstiyorsan numaramız:+905331274743</h3>
                <button id="copyButton">Numarayı Kopyala</button>
             </div>
             
        
        
      </div>
    </section>

   


    

       
  
        
     

    <script>
    const carousel = document.querySelector(".carousel"),
firstImg = carousel.querySelectorAll("img")[0],
arrowIcons = document.querySelectorAll(".wrapper i");

let isDragStart = false, isDragging = false, prevPageX, prevScrollLeft, positionDiff;

const showHideIcons = () => {
    // showing and hiding prev/next icon according to carousel scroll left value
    let scrollWidth = carousel.scrollWidth - carousel.clientWidth; // getting max scrollable width
    arrowIcons[0].style.display = carousel.scrollLeft == 0 ? "none" : "block";
    arrowIcons[1].style.display = carousel.scrollLeft == scrollWidth ? "none" : "block";
}

arrowIcons.forEach(icon => {
    icon.addEventListener("click", () => {
        let firstImgWidth = firstImg.clientWidth + 14; // getting first img width & adding 14 margin value
        // if clicked icon is left, reduce width value from the carousel scroll left else add to it
        carousel.scrollLeft += icon.id == "left" ? -firstImgWidth : firstImgWidth;
        setTimeout(() => showHideIcons(), 60); // calling showHideIcons after 60ms
    });
});

const autoSlide = () => {
    // if there is no image left to scroll then return from here
    if(carousel.scrollLeft - (carousel.scrollWidth - carousel.clientWidth) > -1 || carousel.scrollLeft <= 0) return;

    positionDiff = Math.abs(positionDiff); // making positionDiff value to positive
    let firstImgWidth = firstImg.clientWidth + 14;
    // getting difference value that needs to add or reduce from carousel left to take middle img center
    let valDifference = firstImgWidth - positionDiff;

    if(carousel.scrollLeft > prevScrollLeft) { // if user is scrolling to the right
        return carousel.scrollLeft += positionDiff > firstImgWidth / 2 ? valDifference : -positionDiff;
    }
    // if user is scrolling to the left
    carousel.scrollLeft -= positionDiff > firstImgWidth / 2 ? valDifference : -positionDiff;
}

const dragStart = (e) => {
    // updatating global variables value on mouse down event
    isDragStart = true;
    prevPageX = e.pageX || e.touches[0].pageX;
    prevScrollLeft = carousel.scrollLeft;
}

const dragging = (e) => {
    // scrolling images/carousel to left according to mouse pointer
    if(!isDragStart) return;
    e.preventDefault();
    isDragging = true;
    carousel.classList.add("dragging");
    positionDiff = (e.pageX || e.touches[0].pageX) - prevPageX;
    carousel.scrollLeft = prevScrollLeft - positionDiff;
    showHideIcons();
}

const dragStop = () => {
    isDragStart = false;
    carousel.classList.remove("dragging");

    if(!isDragging) return;
    isDragging = false;
    autoSlide();
}

carousel.addEventListener("mousedown", dragStart);
carousel.addEventListener("touchstart", dragStart);

document.addEventListener("mousemove", dragging);
carousel.addEventListener("touchmove", dragging);

document.addEventListener("mouseup", dragStop);
carousel.addEventListener("touchend", dragStop);


const stopButton = document.getElementById("close-menu-btn");
stopButton.addEventListener("click", function() {
    clearInterval(intervalId);
    carousel.style.display = "none"; // Ana kutuyu gizle
});
// Butonu bulun ve tıklama olayını dinleyin
const copyButton = document.getElementById("copyButton");
copyButton.addEventListener("click", function() {
    const phoneNumber = "+905331274743"; // Kopyalanacak numara
    const tempInput = document.createElement("input");
    tempInput.value = phoneNumber;
    document.body.appendChild(tempInput);
    tempInput.select();
    document.execCommand("copy");
    document.body.removeChild(tempInput);
    alert("Numara başarıyla kopyalandı: " + phoneNumber);
});
const btn = document.querySelector("button");
      const post = document.querySelector(".post");
      const widget = document.querySelector(".star-widget");
      const editBtn = document.querySelector(".edit");
      btn.onclick = ()=>{
        widget.style.display = "none";
        post.style.display = "block";
        editBtn.onclick = ()=>{
          widget.style.display = "block";
          post.style.display = "none";
        }
        return false;
      }
      const header = document.querySelector("header");
      const hamburgerBtn = document.querySelector("#hamburger-btn");
      const closeMenuBtn = document.querySelector("#close-menu-btn");

      // Toggle mobile menu on hamburger button click
      hamburgerBtn.addEventListener("click", () => header.classList.toggle("show-mobile-menu"));

      // Close mobile menu on close button click
      closeMenuBtn.addEventListener("click", () => hamburgerBtn.click());
    </script>
    <script src="script.js"></script>
  </body>
</html>

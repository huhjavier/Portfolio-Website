
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <meta http-equiv="X-UA-Compatible" content="ie=edge">
        <title>Background animation</title>
        <link href="https://fonts.googleapis.com/css?family=Raleway:900" rel="stylesheet">
      </head>
      
      <body>
        <div class="text-container">
          <h1>SAUL BASS</h1>
        </div>
        <div class="where"> <p>Find me here:</p></div>
        <div class="header"><h1>Featured Work</h1></div>
        <div class="home"><a href="/"><h2>HOME</h2></a></div>
        <div class="work"><a href="/work"><h2>WORK</h2></a></div>
        <div class="about"><a href="/about"><h2>ABOUT</h2></a></div>
        <div><a target=”_blank” href="https://www.instagram.com/saul.bass/"><img class="insta" src="insta.svg" alt=""> </a></div>
        <div> <a target=”_blank” href="https://twitter.com/saulbass1920?lang=en"><img class="twitter" src="twitter.svg" alt=""> </a></div>
        <div> <a target=”_blank” href="https://www.facebook.com/saulbassfanpage/"><img class="facebook" src="facebook.svg" alt=""> </a></div>
      </body>
      
</html>


<html lang="en">
    <!DOCTYPE html>
    
    
    <head>
      <meta charset="utf-8" />
      <title>Swiper demo</title>
      <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1, maximum-scale=1" />
      <!-- Link Swiper's CSS -->
      <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css" />
    
      <!-- Demo styles -->
      <style>
        html,
        body {
          position: right;
          height: 100%;
        }
    
        body {
          background: #eee;
          font-family: Helvetica Neue, Helvetica, Arial, sans-serif;
          font-size: 14px;
          color: #000;
          margin: 0;
          padding: 0;
        }
    
        .swiper {
          width: 40%;
          height: 40%;
          position: absolute;
          top: 31%;
          right: 15%;
          
        }
    
        .swiper-slide {
          text-align: center;
          font-size: 18px;
          background: #fff;
          display: flex;
          justify-content: center;
          align-items: center;
        }
    
        .swiper-slide img {
          display: block;
          width: 100%;
          height: 100%;
          object-fit: contain;
        }
    
        .autoplay-progress {
          position: relative;
          right: 16px;
          bottom: 16px;
          z-index: 10;
          width: 48px;
          height: 48px;
          display: flex;
          align-items: right;
          justify-content: right;
          font-weight: bold;
          color: var(--swiper-theme-color);
        }
    
        .autoplay-progress svg {
          --progress: 0;
          position: relative;
          left: 0;
          top: 0px;
          z-index: 10;
          width: 100%;
          height: 100%;
          stroke-width: 4px;
          stroke: var(--swiper-theme-color);
          fill: none;
          stroke-dashoffset: calc(125.6px * (1 - var(--progress)));
          stroke-dasharray: 125.6;
          transform: rotate(-90deg);
        }
      </style>
    </head>
    
    <body>
      <!-- Swiper -->
      <div class="swiper mySwiper">
        <div class="swiper-wrapper">
          <div class="swiper-slide"><img src="armman.jpg" alt=""></div>
          <div class="swiper-slide"><img src="champ.jpg" alt=""></div>
          <div class="swiper-slide"><img src="EXODUS.png" alt=""></div>
          <div class="swiper-slide"><img src="mag7.jpg" alt=""></div>
        </div>
        <div class="swiper-button-next"></div>
        <div class="swiper-button-prev"></div>
        <div class="swiper-pagination"></div>
        <div class="autoplay-progress">
          <svg viewBox="0 0 48 48">
            <circle cx="24" cy="24" r="20"></circle>
          </svg>
          <span></span>
        </div>
      </div>
    
      <!-- Swiper JS -->
      <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
    
      <!-- Initialize Swiper -->
      <script>
        const progressCircle = document.querySelector(".autoplay-progress svg");
        const progressContent = document.querySelector(".autoplay-progress span");
        var swiper = new Swiper(".mySwiper", {
          spaceBetween: 30,
          centeredSlides: true,
          autoplay: {
            delay: 2500,
            disableOnInteraction: false
          },
          pagination: {
            el: ".swiper-pagination",
            clickable: true
          },
          navigation: {
            nextEl: ".swiper-button-next",
            prevEl: ".swiper-button-prev"
          },
          on: {
            autoplayTimeLeft(s, time, progress) {
              progressCircle.style.setProperty("--progress", 1 - progress);
              progressContent.textContent = `${Math.ceil(time / 1000)}s`;
            }
          }
        });
      </script>
    </body>
    
    </html>

<style>
  .where{
    position: absolute;
  top: 3.8%;
  left: 66%;
  color: #FBFBF9;
  font-size: 1.5rem;
  }
  .facebook {
    position: absolute;
    top: 5%;
    left: 81%;
    width: 6%;
    height: 6%;
    filter: invert(100%);
  }
  .facebook:hover{
    transition: all 0.1s ease-out;
filter: invert(20%);
  }
  .insta {position: absolute;
    top: 4.5%;
    left: 73%;
    width: 7%;
    height: 7%;
    filter: invert(100%);
  }
  .insta:hover{
    transition: all 0.1s ease-out;
filter: invert(20%);
  }
  .twitter {
    position: absolute;
    top: 4.5%;
    left: 77%;
    width: 7%;
    height: 7%;
    filter: invert(100%);
  }
  .twitter:hover{
    transition: all 0.1s ease-out;
    filter: invert(20%);
  }

   .header {
  position: absolute;
  top: 24%;
  right: 30%;
  color: #FBFBF9;
}
.home {
  position: absolute;
  top: 25.5%;
  left: 10%;
  color: #FBFBF9;
  font-size: 2.2rem;

}
.work {
  position: absolute;
  top: 43.5%;
  left: 10%;
  color: #FBFBF9;
  font-size: 2.2rem;
}
.about {
  position: absolute;
  top: 60.5%;
  left: 10%;
  color: #FBFBF9;
  font-size: 2.2rem;
}

a {
  text-decoration: none;
  color: #FBFBF9;
}

    body {
  margin: 0;
  padding: 0;
  font-family: 'Raleway', sans-serif;
  background-color: #000;
}

.text-container {
  height: 100vh;
  width: 100vw;
  display: flex;
  justify-content: top;
  align-items: top;
}

h2:hover {
transition: all 0.1s ease-out;
filter: brightness(50%);
} 

.text-container h1{
  margin: 0;
  font-size: 150px;
  color: rgba(225,225,225, .01);
  background-image: url("https://lallsopp.github.io/john_baskerville/images/saul-bass-posters.jpg");
  background-repeat: repeat;
  background-clip:text;
  animation: animate 15s ease-in-out infinite;
  text-align: top;
  text-transform: uppercase;
  font-weight: 900;
}

  @keyframes animate {
    0%, 100% {
      background-position: left top;
    }
    25%{
      background-position: right bottom;
     }
    50% {
      background-position: left bottom;
    }
    75% {
      background-position: right top;
    }   
}
</style>
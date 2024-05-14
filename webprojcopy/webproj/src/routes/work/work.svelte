<script>
  import { base } from '$app/paths'
</script>
<html lang="en">
 <body>
    <div><a href="{base}/"><img class="home" src="bxs-home.svg" alt=""></a></div>
 </body>   
</html>
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="utf-8" />
  <title>Swiper demo</title>
  <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1, maximum-scale=1" />
  <!-- Link Swiper's CSS -->
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css" />
  <link href="https://fonts.googleapis.com/css?family=Raleway:900" rel="stylesheet">

  <!-- Demo styles -->
  <style>
    .home{
    position: absolute;
    top: 86%;
    left: 0.5%;
    width: 10%;
    height: 10%;
    filter: invert(100%);
  }
    html,
    body {
      position: relative;
      height: 100%;
      background-color: black;
    }

    body {
      font-family: Helvetica Neue, Helvetica, Arial, sans-serif;
      font-size: 14px;
      color: #000;
      background-color: black;
      margin: 0;
      padding: 0;
    }

    .swiper {
      width: 100%;
      padding-top: 50px;
      padding-bottom: 50px;
    }

    .swiper-slide {
      background-position: center;
      background-size: cover;
      width: 300px;
      height: 500px;
    }

    .swiper-slide img {
      display: block;
      width: 100%;
    }
  </style>
</head>

<body>
  <!-- Swiper -->
  <div class="swiper mySwiper">
    <div class="swiper-wrapper">
      <div class="swiper-slide">
        <img src="https://www.indiewire.com/wp-content/uploads/2017/08/edge_bass.png?w=455" alt="">
      </div>
      <div class="swiper-slide">
        <img src="https://www.indiewire.com/wp-content/uploads/2017/08/stjoan_bass.jpg?w=450" alt="" />
      </div>
      <div class="swiper-slide">
        <img src="https://www.indiewire.com/wp-content/uploads/2017/08/love_bass.png?w=457" alt=""/>
      </div>
      <div class="swiper-slide">
        <img src="https://www.indiewire.com/wp-content/uploads/2017/08/vertigo.jpg?w=466" alt=""/>
      </div>
      <div class="swiper-slide">
        <img src="https://www.indiewire.com/wp-content/uploads/2017/08/bigcountry_bass.png?w=461" alt=""/>
      </div>
      <div class="swiper-slide">
        <img src="https://www.indiewire.com/wp-content/uploads/2017/08/bonjour_bass.png?w=500" alt=""/>
      </div>
      <div class="swiper-slide">
        <img src="https://www.indiewire.com/wp-content/uploads/2017/08/anatomy_bass_alt.png?w=501" alt=""/>
      </div>
      <div class="swiper-slide">
        <img src="https://www.indiewire.com/wp-content/uploads/2017/08/magnificent2_bass.jpg?w=450" alt=""/>
      </div>
      <div class="swiper-slide">
        <img src="https://www.indiewire.com/wp-content/uploads/2017/08/spartacus_bass.png?w=423" alt=""/>
      </div>
    </div>
    <div class="swiper-pagination"></div>
  </div>

  <!-- Swiper JS -->
  <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>

  <!-- Initialize Swiper -->
  <script>
    var swiper = new Swiper(".mySwiper", {
      effect: "coverflow",
      grabCursor: true,
      centeredSlides: true,
      slidesPerView: "auto",
      coverflowEffect: {
        rotate: 50,
        stretch: 0,
        depth: 100,
        modifier: 1,
        slideShadows: true,
      },
      pagination: {
        el: ".swiper-pagination",
      },
    });
  </script>
</body>

</html>

<style>
    html {
        background-color: black;
    }
</style>
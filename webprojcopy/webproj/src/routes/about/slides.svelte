<script>
  import { base } from '$app/paths'
</script>
<html lang="en">
  <body>
    <div class="ripple background">
      <div class="circle small shade1"></div>
      <div class="circle medium shade2"></div>
      <div class="circle large shade3"></div>
    </div>
    <div class="about"><h1>About the artist</h1></div>
    <a href="{base}/"><img class="home" src="bxs-home.svg" alt=""></a>
    <div> <img class="dude" src="https://lallsopp.github.io/john_baskerville/images/Saul%20Bass%20portrait.jpg" alt="saul"></div>
    <div class="who"><p>Saul Bass was born in The Bronx, New York on 8th May 1920 to Eastern European Jewish immigrant parents.
       He began drawing from an early age and went on to graduate from James Monroe high school.
       He attended the Art students League in Manhattan part-time until going on to attend night classes at Brooklyn college with György Kepes (a famous Hungarian designer).
       After completing his studies, he worked as a freelance designer before moving to Hollywood and becoming a commercial artist.
      In the 1940’s Bass began his time in Hollywood. He started to create movie posters, corporate logos and later went on to make movie title sequences. In 1952 he established his own firm “Saul Bass and Associates”.</p></div>
      <div class="quote"><p>“if it’s simple simple, it’s boring… we try for the idea that is so simple that it will make you think and rethink” —Saul Bass</p></div>
  </body>
  <link href="https://fonts.googleapis.com/css?family=Raleway:900" rel="stylesheet">
</html>

<style>
  html {
    max-height: 100%;
  }
  .quote{
    position: absolute;
  top: 65%;
  left: 60%;
  right: 15%;
  color: #FBFBF9;
  font-size: 1rem;
  font-family: raleway;
  text-align: left;
    display: block;
    margin: 20px auto;
  }
  .home{
    position: absolute;
    top: 86%;
    left: 0.5%;
    width: 10%;
    height: 10%;
  }
  .dude{
   position: absolute;
   top: 30%;
   right: 45%;
   width: 20%;
   height: 30%;

  }
  .about{
    position: absolute;
  top: 10%;
  right: 25%;
  color: #FBFBF9;
  font-size: 2rem;
  font-family: raleway;
  }
  .who{
    position: absolute;
  top: 25%;
  left: 60%;
  right: 15%;
  color: #FBFBF9;
  font-size: 1rem;
  font-family: Helvetica Neue, Helvetica, Arial, sans-serif;
  text-align: center;
    display: block;
    margin: 20px auto;
  }

  body{
    background: #000000;
    max-height: 100%;
  }
  .circle{
position: absolute;
border-radius: 50%;
background: #fff;
animation: ripple 10s infinite;
box-shadow: 0px 0px 1px 0px #000000;
  }
    .small{
      width: 600px;
      height: 600px;
      left: -300px;
      bottom: -300px;
    }
    .medium{
      width: 800px;
      height: 800px;
      left: -400px;
      bottom: -400px;
    }
    .large{
      width: 1000px;
      height: 1000px;
      left: -500px;
      bottom: -500px;
    }

    .shade1{
      opacity: 0.7;
    }
    .shade2{
      opacity: 0.5;
    }
    .shade3{
      opacity: 0.2;
    }
    @keyframes ripple{
      0%{
        transform: scale(0.8);
      }
      50%{
        transform: scale(1.2);
      }
      100%{
        transform: scale(0.8);
      }
    }
</style>
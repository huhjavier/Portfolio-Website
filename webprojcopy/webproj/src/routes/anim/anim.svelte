<link
rel="stylesheet"
href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css"
/>
<html lang="en">
    <section>
        <div class="swiper mySwiper">
            <div class="swiper-wrapper">
                <div class="swiper-slide">
                    <div class="TestimonialBox">
                        <!-- svelte-ignore a11y-missing-attribute -->
                        <img src="quote.png" class="quote">
                        <div class="content">
                            <p>Lorem ipsum dolor sit amet consectetur 
                            adipisicing elit. Natus, eum!</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
</html>
<script>
    import { onMount } from 'svelte';

    onMount(() => {
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
    }) 
</script>
<style>
    @import url('https://fonts.googleapis.com/css?family=Poppins:200,300,400,500,600,700,800,900&disp');
    *{
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
    }
    section {
        position: relative;
        width: 100%;
        min-height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        background: #2196f3;
        overflow: hidden;
    }
.swiper 
{
 width: 100%;
 padding-top: 50px;
 padding-bottom: 50px;
}

.swiper-slide 
{
 background-position: center;
 background-size: cover;
 width: 300px;
 height: 300px;
}
</style>
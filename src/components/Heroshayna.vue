<template>
    <!-- Hero Section Begin -->
    <section class="hero-section">
        <carousel class="hero-items" :items="1" :nav="false" :autoplay="true">
            
            <div class="single-hero-items set-bg" style="background-image : url('/img/hero-jordans.jpg')">
                <div class="container">
                    <div class="row">
                        <div class="col-lg-5">
                            <span>Sneakers,Nike</span>
                            <h1>Air Jordan Collections</h1>
                            <p>
                                
                            </p>
                            <a href="#" class="primary-btn">Shop Now</a>
                        </div>
                    </div>
                </div>
            </div>
           <div class="single-hero-items set-bg" style="background-image : url('/img/hero-cfog.jpg')">
                <div class="container">
                    <div class="row">
                        <div class="col-lg-5">
                            <span>Sneakers,Converse</span>
                            <h1>Converse x FOG</h1>
                            <p>
                                
                            </p>
                            <a href="#" class="primary-btn">Shop Now</a>
                        </div>
                    </div>
                </div>
            </div>
            <div class="single-hero-items set-bg" style="background-image : url('/img/hero-jersey.jpg')">
                <div class="container">
                    <div class="row">
                        <div class="col-lg-5">
                            <span>Football Kit</span>
                            <h1>Vintage Football Kit</h1>
                            <p>
                                
                            </p>
                            <a href="#" class="primary-btn">Shop Now</a>
                        </div>
                    </div>
                </div>
            </div>
        </carousel>
    </section>
    <!-- Hero Section End -->
</template>

<script>
import carousel from "vue-owl-carousel";
export default {
    name: "Heroshayna",
    components: {
        carousel
    }
}
</script>
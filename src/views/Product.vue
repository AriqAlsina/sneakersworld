<template>
  <div class="product">
  <HeaderShayna/>
  <!-- Breadcrumb Section Begin -->
    <div class="breacrumb-section text-left">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="breadcrumb-text product-more">
                        <router-link to="/"><i class="fa fa-home"></i> Home</router-link>
                        <span>Detail</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- Breadcrumb Section Begin -->

    <!-- Product Shop Section Begin -->
    <section class="product-shop spad page-details">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="row">
                        <div class="col-lg-6">
                            <div class="product-pic-zoom">
                                <img class="product-big-img" :src="gambar_default" alt="" />
                            </div>
                            <div class="product-thumbs">
                                <carousel :dots="false" :nav="false"
                                class="product-thumbs-track ps-slider">
                                    <div class="pt" @click="changeImage(thumbs[0])" :class="thumbs[0] == gambar_default ? 'active' : '' ">
                                        <img src="img/products/nike-01.jpg" alt="" />
                                    </div>

                                    <div class="pt" @click="changeImage(thumbs[1])" :class="thumbs[1] == gambar_default ? 'active' : '' ">
                                        <img src="img/products/nsbdp-01.jpg" alt="" />
                                    </div>

                                    <div class="pt" @click="changeImage(thumbs[2])" :class="thumbs[2] == gambar_default ? 'active' : '' ">
                                        <img src="img/products/nsbdp-02.jpg" alt="" />
                                    </div>
                                </carousel>
                            </div>
                        </div>
                        <div class="col-lg-6">
                            <div class="product-details text-left">
                                <div class="pd-title">
                                    <span>Sneakers</span>
                                    <h3>NIKE SB DUNK LOW PARRA</h3>
                                </div>
                                <div class="pd-desc">
                                    <p>
                                         Piet Parra‘s newest foray with Beaverton is one met with a balance of both color and neutrals. Choosing the Nike SB Dunk Low as his canvas, the Amsterdam-based artist is readied to dose in his quiet vibrant motifs onto the silhouette. Plain white leathers comprise the majority of the construction — lending itself to pleasing distressing once worn as intended — while much of the eye draws to the focal profile swooshes, which forgo the traditional overlay for a tripled chenille of blue to red, to pink. Small embroidered miniature checks sit along the forefoot with the lining being the most loudest feature as its mosaic of geometric shapes and loud hues is unabashed in its execution. Playful logo lock-ups finish up with both partners right on the heel for a pair that slowly welcomes back the collaborator into the midst of the current market.
                                    </p>
                                    <h4>Rp 4.500.000</h4>
                                </div>
                                <div class="quantity">
                                    <router-link to="/cart"><a href="shopping-cart.html" class="primary-btn pd-cart">Add To Cart</a></router-link>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- Product Shop Section End --> 
  <RelatedShayna/>
  <FooterShayna/>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
import HeaderShayna from "@/components/Headershayna.vue";
import FooterShayna from "@/components/Footershayna.vue";
import carousel from "vue-owl-carousel";
import RelatedShayna from "@/components/Relatedshayna.vue";

export default {
  name: "Product",
  components: {
    HeaderShayna,
    FooterShayna,
    carousel,
    RelatedShayna
  },
  data() {
      return {
       gambar_default: "img/products/nike-01.jpg",
       thumbs: [
           "img/products/nike-01.jpg",
           "img/products/nsbdp-01.jpg",
           "img/products/nsbdp-02.jpg",
       ]
      }
  },
  methods: {
      changeImage(urlImage) {
          this.gambar_default = urlImage;
  }
  }
};
</script>

<style scoped>
.product-thumbs .pt {
    margin-right: 14px;
}
</style>
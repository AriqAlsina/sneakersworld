<template>
  <div class="home">
  <HeaderShayna/> 
  <HeroShayna/>
  <WomenBannerShayna/>
  <InstaShayna/>
  <PartnerShayna/>
  <FooterShayna/>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
import HeaderShayna from "@/components/Headershayna.vue";
import HeroShayna from "@/components/Heroshayna.vue";
import WomenBannerShayna from "@/components/Womenbannershayna.vue";
import InstaShayna from "@/components/Instashayna.vue";
import PartnerShayna from "@/components/Partnershayna.vue";
import FooterShayna from "@/components/Footershayna.vue";



export default {
  name: "Home",
  components: {
    HeaderShayna,
    HeroShayna,
    WomenBannerShayna,
    InstaShayna,
    PartnerShayna,
    FooterShayna
  }
}
</script>

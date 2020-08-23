<template>
    <!-- Women Banner Section Begin -->
    <section class="women-banner spad">
        <div class="container-fluid">
            <div class="row">
                <div class="col-lg-12 mt-5">
                    <carousel class="product-slider" :items="3" :dots="false" :nav="false" :autoplay="true">
                        <div class="product-item">
                            <div class="pi-pic">
                                <img src="img/products/nike-01.jpg" alt="" />
                                <ul>
                                    <li class="w-icon active">
                                        <a href="#"><i class="icon_bag_alt"></i></a>
                                    </li>
                                    <li class="quick-view">
                                        <router-link to="/product">+ Quick View</router-link>
                                        </li>
                                </ul>
                            </div>
                            <div class="pi-text">
                                <div class="catagory-name">Sneakers</div>
                                <router-link to="/product">
                                <a href="#">
                                    <h5>Nike SB Dunk Low Parra</h5>
                                </a>
                                </router-link>
                                <div class="product-price">
                                    Rp 4.500.000
                                </div>
                            </div>
                        </div>
                        <div class="product-item">
                            <div class="pi-pic">
                                <img src="img/products/nike-02.jpg" alt="" />
                                <ul>
                                    <li class="w-icon active">
                                        <a href="#"><i class="icon_bag_alt"></i></a>
                                    </li>
                                    <li class="quick-view"><a href="#">+ Quick View</a></li>
                                </ul>
                            </div>
                            <div class="pi-text">
                                <div class="catagory-name">Sneakers</div>
                                <a href="#">
                                    <h5>Nike Air Jordan 1 Mid Light Smoke Grey</h5>
                                </a>
                                <div class="product-price">
                                    Rp 2.500.000
                                </div>
                            </div>
                        </div>
                        <div class="product-item">
                            <div class="pi-pic">
                                <img src="img/products/adidas-01.jpg" alt="" />
                                <ul>
                                    <li class="w-icon active">
                                        <a href="#"><i class="icon_bag_alt"></i></a>
                                    </li>
                                    <li class="quick-view"><a href="#">+ Quick View</a></li>
                                </ul>
                            </div>
                            <div class="pi-text">
                                <div class="catagory-name">Sneakers</div>
                                <a href="#">
                                    <h5>Adidas NMD Hu Pharrell x BBC Blue Plaid</h5>
                                </a>
                                <div class="product-price">
                                    Rp 4.400.000
                                </div>
                            </div>
                        </div>
                        <div class="product-item">
                            <div class="pi-pic">
                                <img src="img/products/converse-01.jpg" alt="" />
                                <ul>
                                    <li class="w-icon active">
                                        <a href="#"><i class="icon_bag_alt"></i></a>
                                    </li>
                                    <li class="quick-view"><a href="#">+ Quick View</a></li>
                                    <li class="w-icon">
                                        <a href="#"><i class="fa fa-random"></i></a>
                                    </li>
                                </ul>
                            </div>
                            <div class="pi-text">
                                <div class="catagory-name">Sneakers</div>
                                <a href="#">
                                    <h5>Converse Chuck Taylor All-Star 70s Hi Fear of God Cream</h5>
                                </a>
                                <div class="product-price">
                                    Rp 5.500.000
                                </div>
                            </div>
                        </div>
                    </carousel>
                </div>
            </div>
        </div>
    </section>
    <!-- Women Banner Section End -->
</template>

<script>
import carousel from "vue-owl-carousel";
export default {
    name: "Womenbannershayna",
    components: {
        carousel
    }
}
</script>

<style scoped>
.product-item {
    margin-right: 25px;
}
</style>
<template>
    <div class="hero-ebook hero-swiper-btn" id="home">
        <div class="container_f1">
            <div class="swiper-wrapper">
                <swiper
                    :speed="1000"
                    :loop="true"
                    :navigation="swiperOptions.navigation"
                >
                    <swiper-slide class="swiper-slide" :style="bgImg">
                        <div class="hero-item">
                            <div class="hero-content">
                                <h6 class="hero-content-subtitle">It's time for stablecoins</h6>
                                <h2 class="hero-content-title">National stablecoins on blockchain</h2>
                                <p>The idea behind Stabilitas is to provide a stable and secure digital asset that can be used for various purposes such as making purchases, remittances, and as a store of value.</p>
                            </div>
                        </div>
                    </swiper-slide>

                    <!-- Optional controls -->
                    <div class="swiper-button-prev swiper-button-white">
                        <i class="fas fa-chevron-left"></i>
                    </div>
                    <div class="swiper-button-next swiper-button-white">
                        <i class="fas fa-chevron-right"></i>
                    </div>
                </swiper>
            </div>
        </div>
    </div>
</template>

<script>
    import { Swiper, SwiperSlide } from "swiper/vue"
    import SwiperCore, { Navigation } from 'swiper/core'
    SwiperCore.use([Navigation])

    import "swiper/css"

    export default {
        components: {
            Swiper,
            SwiperSlide
        },

        data() {
            return {
                bgImg: {
                    backgroundImage: `url(${require("../assets/img/hero/ebook/ebook-hero-bg.jpg")})`
                },
                swiperOptions: {
                    navigation: {
                        nextEl: '.swiper-button-next',
                        prevEl: '.swiper-button-prev'
                    },
                }
            };
        }
    };
</script>

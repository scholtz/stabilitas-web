<template>
    <div class="cta-image-area_one section-space--ptb_120">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="cta-image cta-image-bg bg-cover">
                        <div class="row align-items-center">
                            <div class="col-lg-6 order-2 order-lg-1">
                                <div class="cta-image__content">
                                    <h4 class="cta-image__title text-white mb-20 wow move-up">Free download of our app now</h4>
                                    <div class="cta-image__text text-white mb-20 wow move-up">Offer your business with the best assistance for growth.</div>
                                    <router-link :to="{ path: 'branding' }" class="btn btn--green">
                                        <span class="btn-icon  ml-0 mr-2"><i class="fa fa-arrow-alt-to-bottom"></i></span> Get Stabilitas
                                    </router-link>
                                </div>
                            </div>
                            <div class="col-lg-6 order-1 order-lg-2">
                                <div class="cta-image__media wow move-up">
                                    <img src="../assets/img/banners/stabilitas-macbook-01.png" class="img-fluid" alt="stabilitas-macbook-01">
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'CtaOne',
    }
</script>
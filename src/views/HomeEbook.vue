<template>
    <div class="main-container box-page">
        <div class="site-wrapper-box">
            <div class="site-wrapper">
                <HeaderEbook />
                <HeroEbook />
                <EbookIntro />
                <CtaThree id="whitepaper" />
                <EBookFAQ />
                <FooterBottom />
                <OffcanvasSearchBox />
            </div>
        </div>
    </div>
</template>

<script>
    import HeaderEbook from '@/components/HeaderEbook'
    import HeroEbook from '@/components/HeroEbook'
    import EbookIntro from '@/components/sections/EbookIntro'
    import EbookChanters from '@/components/sections/EbookChanters'
    import EbookTestimonial from '@/components/sections/EbookTestimonial'
    import CtaThree from '@/components/CtaThree'
    import EbookMailchimp from '@/components/sections/EbookMailchimp'
    import FooterBottom from '@/components/FooterBottom'
    import OffcanvasSearchBox from '@/components/OffcanvasSearchBox'
    import EBookFAQ from '@/components/EBookFAQ'

    export default {
        name: 'HomeEbook',
        components: {
            HeaderEbook,
            HeroEbook,
            EbookIntro,
            EbookChanters,
            EbookTestimonial,
            CtaThree,
            EbookMailchimp,
            FooterBottom,
            EBookFAQ,
            OffcanvasSearchBox
        }
    }
</script>
<template>
    <div class="ebook-feature section-space--pt_120 section-space--pb_60" id="intro">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="section-title-wrapper text-center section-space--mb_60">
                        <h2 class="section-title font-weight--blod wow move-up">We deliver the smart contracts to issue stablecoins on Algorand</h2>
                    </div>
                </div>
            </div>
            <!-- ebook features component -->
            <div class="row">
                <div class="col-lg-6">
                    <div class="section-title-wrapper text-center section-space--mb_60">
                        <YouTube 
                            src="https://www.youtube.com/watch?v=cSJjmnzvvLY" 
                            @ready="onReady"
                            ref="youtube" />
                    </div>
                </div>
                <div class="col-lg-6">
                    <div class="section-title-wrapper text-center section-space--mb_60">
                        <h3>Greenhouse hack #3</h3>
                        <p>
                            Project Stabilitas has been created @ Greenhouse hack #3
                        </p>
                        <p><a href="https://gitcoin.co/issue/29663" target="_blank">https://gitcoin.co/hackathon/greenhouse3/</a></p>
                        <p>During the hackathon: </p>
                        <div class="pricing-table__inner">
                    <div class="pricing-table__body"><ul class="pricing-table__list text-left"><li>the project has been thought through, </li><li>the Whitepaper has been written, </li><li>and MVP has been deployed to the algorand testnet.</li>
                        <li>Two open source github repos has been created:</li>
                        <li><a href="https://github.com/scholtz/stabilitas-apps" target="_blank">https://github.com/scholtz/stabilitas-apps</a></li>
                        <li><a href="https://github.com/scholtz/stabilitas-web" target="_blank">https://github.com/scholtz/stabilitas-web</a></li>
                        </ul></div>
                    </div></div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import EbookFeature from '@/components/EbookFeature'
    import YouTube from 'vue3-youtube'

    export default {
        name: 'EbookIntro',
        components: {
            EbookFeature,YouTube
        }
    };
</script>
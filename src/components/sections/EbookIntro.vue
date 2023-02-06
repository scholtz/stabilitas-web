<template>
    <div class="ebook-feature " id="intro">
        <div class="container section-space--pt_120 section-space--pb_60">
            <div class="row">
                <div class="col-lg-12">
                    <div class="section-title-wrapper text-center section-space--mb_60 section-space--pt_120">
                        <h2 class="section-title font-weight--blod wow move-up">We delivered the proof of concept to issue stablecoins on Algorand using smart contracts</h2>
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
                        <div class="pricing-table__body">
                            <ul class="pricing-table__list text-left"><li>the project has been thought through, </li><li>the <b><a href="/white-paper-stabilitas-20230206.pdf" target="_blank">Whitepaper</a></b> has been written, </li><li>and PoC has been deployed to the algorand testnet.</li>
                                <li>Two open source github repos has been created:</li>
                                <li><a href="https://github.com/scholtz/stabilitas-apps" target="_blank">https://github.com/scholtz/stabilitas-apps</a></li>
                                <li><a href="https://github.com/scholtz/stabilitas-web" target="_blank">https://github.com/scholtz/stabilitas-web</a></li>
                            </ul>
                        </div>
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
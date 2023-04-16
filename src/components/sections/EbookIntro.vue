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
                            src="https://www.youtube.com/watch?v=VyQsf0ePhL8" 
                            @ready="onReady"
                            ref="youtube" />
                    </div>
                </div>
                <div class="col-lg-6">
                    <div class="section-title-wrapper text-center section-space--mb_60">
                        <h3>Mega Ace Hackathon</h3>
                        <p>
                            Project Stabilitas has been <br/>deployed to testnet @ Mega Ace Hackathon
                        </p>
                        <p><a href="https://mega-ace.org/hackathon" target="_blank">https://mega-ace.org/hackathon</a></p>
                        <pre>tokensAppId=194446915
assetOracleBase=37074699
oracleECBAppId=194448390
oracleAMMVWAP1W=194448649
oracleAMMVWAP1H=194448614
reserveAppId=194449294
</pre>
                    </div>
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
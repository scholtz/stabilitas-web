<template>
    <div class="ebook-feature section-space--pt_120 section-space--pb_60" id="faq">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="section-title-wrapper text-center section-space--mb_60">
                        <h2 class="section-title font-weight--blod wow move-up">Frequently asked questions</h2>
                    </div>
                </div>
            </div>
            <!-- ebook features component -->
            <Accordion />
        </div>
    </div>
</template>

<script>
    import Accordion from '@/components/Accordion'

    export default {
        name: 'EbookFAQ',
        components: {
            Accordion
        }
    };
</script>
<template>
    <div>
        <div class="container">
            <div class="row mt-5">
                <h3>Você está vendo notícias do {{ championship }}</h3>
            </div>
        </div>
        <HcodeSectionBanner/>
        <HcodeSectionNews/>
        <div class="container">
            <div class="row my-club mt-05">
                <div class="col-6">
                    <h2>Seu Clube é: {{ myClub }}</h2>
                </div>
                <div class="col-6">
                    <HcodeInput v-model="myClub"/>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import HcodeSectionBanner from './HcodeSectionBanner.vue';
import HcodeSectionNews from './HcodeSectionNews.vue';
import HcodeInput from './HcodeInput.vue';
export default {
    components: {
        HcodeSectionBanner,
        HcodeSectionNews,
        HcodeInput
    },
    data() {
        return {
            myClub: 'Hcode Treinamentos'
        }
    },
    props: {
        championship: String
    }
}
</script>
<style scoped>

</style>
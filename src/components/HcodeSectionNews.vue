<template>
    <section>
        <div class="container">
            <HcodeSectionNewsIndividual img-name="" img-info="" news-title="" news-content="" news-date=""/>

            <HcodeSectionNewsIndividual img-name="news2.jpg" img-info="Notícia 2" news-title="Jogo de quarta-feira termina empatado" news-content="Lorem ipsum dolor sit amet consectetur, adipisicing elit. Illum assumenda exercitationem, aperiam ea, voluptas ipsa quae cumque nobis aliquam, quos doloremque harum voluptatum qui doloribus consequatur. Nobis velit excepturi aliquam!" news-date="27/12/2023"/>

            <HcodeSectionNewsIndividual img-name="news3.jpg" img-info="Notícia 3" news-title="A inauguração do novo estádio será na semana que vem" news-content="Lorem ipsum dolor sit amet consectetur, adipisicing elit. Illum assumenda exercitationem, aperiam ea, voluptas ipsa quae cumque nobis aliquam, quos doloremque harum voluptatum qui doloribus consequatur. Nobis velit excepturi aliquam!" news-date="30/12/2023"/>
        </div>
    </section>
</template>
<script>
import HcodeSectionNewsIndividual from './HcodeSectionNewsIndividual.vue';
export default {
    components: {
        HcodeSectionNewsIndividual
    },
    data() {
        return {
            news: []
        }
    },
    created() {
        this.news[{
            id: 1,
            title: 'Começam os treinos para a nova temporada',
            content: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Illum assumenda exercitationem, aperiam ea, voluptas ipsa quae cumque nobis aliquam, quos doloremque harum voluptatum qui doloribus consequatur. Nobis velit excepturi aliquam!',
            date: '2020-01-01',
            img: 'news1.jpg',
            imgInfo: 'Notícia 1'
        }]
    }
}
</script>
<style scoped>
section {
    padding: 50px 0;
    margin-top: 25px;
    background-color: #F37520;
}
</style>
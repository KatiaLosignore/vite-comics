<script>
import AppBottom from './AppBottom.vue';
export default {
    name: 'AppMain',
    components: { AppBottom },
    props: {
        cards: Array
    }
};

</script>

<template>
    <main id="comics">
        <section id="jumbutron">
        </section>
        <div class="container">
            <section id="cards">
                
                <ul>
                    <li v-for="card in cards" :key="card.series">
                        <img :src="card.thumb" :alt="card.type">
                        <p>{{ card.series }}</p>
                    </li>
                </ul>

                <app-bottom></app-bottom>
            
            </section>
        </div>
    </main>


</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
@use '../assets/scss/partials/mixins' as *;

    #comics {
        background-color: $black;
        height: 960px;
    }

   #cards {
    padding-top: 30px;
   }

    ul {
        @include center_flex;
        flex-wrap: wrap;
        margin: 8px 0;
        gap: 15px;

        li {
            list-style-type: none;
            font-weight: bold;
            font-size: 13px;
            color: $white;
            text-transform: uppercase;
            width: 15%;
            margin: 10px 0;
        }

            img {
                width: 200px;
                height: 200px;
            }

            p {
                font-size: 10px;
                margin-top: 8px;
            }
           
    }

    #jumbutron {
        background-image: url('../assets/img/jumbotron.jpg');
        background-size: cover;
        background-position: top;
        height: 320px;
    }

</style>
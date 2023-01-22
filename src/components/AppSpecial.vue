<script>
    export default {
        name: 'AppSpecial',
        data() {
            return {
                images: [
                    { id: 1, text: 'digital comics', url: '#', image: 'buy-comics-digital-comics.png' },
                    { id: 2, text: 'dc merchandise', url: '#', image: 'buy-comics-merchandise.png' },
                    { id: 3, text: 'subscription', url: '#', image: 'buy-comics-subscriptions.png' },
                    { id: 4, text: 'comic shop locator', url: '#', image: 'buy-comics-shop-locator.png' },
                    { id: 5, text: 'dc power visa', url: '#', image: 'buy-dc-power-visa.svg' }, 

                ],
            }
        },
        methods: {
            buildImagePath(image) {
                const url = new URL(`../assets/img/${image.image}`, import.meta.url);
                return url.href;
            }
        }
    };             
</script>        

<template>
    <div>
        <ul>
            <li v-for="image in images" :key="image.id">
                <a :href="image.url">
                    <img :src="buildImagePath(image)" :class="{'img-width' : image.id === 4, 'img-first' : image.id === 1, 'img-last' : image.id === 5}">
                    <p>{{image.text}}</p>
                </a>
            </li>
        </ul>

    </div>

</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/mixins' as *;
@use '../assets/scss/partials/variables' as *;

    div {
        position: relative;
        z-index: 2;
        background-color: $blue;
        height: 130px;
    }

    ul {
        @include center_flex;
        padding: 0;

        li {
            list-style-type: none;
            font-weight: bold;
            font-size: 13px;
            padding: 28px;

            a {
                @include center_flex;
                padding: 10px;
                text-transform: uppercase;
                color: $white;
                font-size: 12px;
            }
        }
    }

    img {
        width: 50px;
        margin-right: 10px;
        object-fit: cover;
    }

    .img-width {
        width : 30px;
    }

    .img-first {
        width: 40px;
    }

    .img-last {
        width: 55px;
    }
</style>
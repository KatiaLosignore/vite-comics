<script>
    export default {
        name: 'AppSpecial',
        data() {
            return {
                images: [
                    { text: 'digital comics', url: '#', image: 'buy-comics-digital-comics.png' },
                    { text: 'dc merchandise', url: '#', image: 'buy-comics-merchandise.png' },
                    { text: 'subscription', url: '#', image: 'buy-comics-subscriptions.png' },
                    { text: 'comic shop locator', url: '#', image: 'buy-comics-shop-locator.png' },
                    { text: 'dc power visa', url: '#', image: 'buy-dc-power-visa.svg' },

                ]
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
            <li v-for="image in images" :key="image.text">
                <a :href="image.url">
                    <img :src="buildImagePath(image)">
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
        height: 150px;
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
        width: 45px;
        margin-right: 10px;
        object-fit: cover;
    }
</style>
<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            links: [
                { text: 'Characters', url: '#', current: false },
                { text: 'Comics', url: '#', current: true },
                { text: 'Movies', url: '#', current: false },
                { text: 'TV', url: '#', current: false },
                { text: 'Games', url: '#', current: false },
                { text: 'Collectibles', url: '#', current: false },
                { text: 'Videos', url: '#', current: false },
                { text: 'Fans', url: '#', current: false },
                { text: 'News', url: '#', current: false },
                { text: 'Shop', url: '#', current: false },
            ]
        }
    }
};

</script>

<template>
    <div class="container">

        <header>
            
            <nav>
                <a href="#"><img src="../assets/img/dc-logo.png" alt="logo"></a>
                <ul>
                    <li v-for='link in links' :key="link.text">
                        <a :href='link.url' v-text="link.text" :class="{ 'active': link.current }"></a>
                    </li>
                </ul>
            </nav>
        </header>

    </div>

</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/mixins' as *;
@use '../assets/scss/partials/variables' as *;
   

    nav {
        display: flex;
        justify-content: space-between;
    }

    header {
        padding-top: 20px;
        height: 150px;
    }

    ul {
        @include center_flex;
        margin: 30px;
        padding: 0;

        li {
            list-style-type: none;
            font-weight: bold;
            font-size: 13px;

            a {
                padding: 10px;
                text-transform: uppercase;

                &.active {
                    color: $blue;
                    padding-bottom: 65px;
                    border-bottom: 4px solid $blue;
                }
            }

        }


    }


</style>

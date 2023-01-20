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
    <header>
        <figure>
            <a href="#"><img src="../assets/img/dc-logo.png" alt="logo"></a>
        </figure>
        <nav>
            <ul>
                <li v-for='link in links' :key="link.text">
                    <a :href='link.url' v-text="link.text" :class="{ 'active': link.active }"></a>
                </li>
            </ul>
        </nav>
    </header>

</template>

<style scoped>
    ul {
        display: flex;
        justify-content: center;
        align-items: center;
        margin: 30px;
        padding: 0;
    }

    ul li {
        list-style-type: none;
        font-weight: bold;
    }

    ul li a {
        padding: 10px;
    }

    ul li a.active {
        color: blue;
    }
</style>

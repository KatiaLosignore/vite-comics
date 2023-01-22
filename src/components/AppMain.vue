<script>
export default {
    name: 'AppMain'
};

</script>

<template>
    <main id="comics">
        <div class="container">
            <section>
                <h2>Content goes here</h2>
            </section>
        </div>
    </main>


</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

    #comics {
        background-color: $black;
        height: 110px;
    }

    h2{
        color: $white;
        padding: 35px;
    }

</style>
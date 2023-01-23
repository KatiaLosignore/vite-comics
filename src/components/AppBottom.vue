<script>
export default {
    name: 'AppBottom'
};

</script>

<template>
    <div class="buttons">
        <div class="load-button">LOAD MORE</div>
    </div>
  
</template>


<style  lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.buttons {
    margin: 25px auto;
    padding: 14px;
    width: 160px;
    border-radius: 18px;
    font-size: 11px;
    font-weight: 600;
    cursor: pointer;

    .load-button {
        background-color: $blue;
        padding: 10px;
        color: $white;
        text-align: center;
    }
}

</style>
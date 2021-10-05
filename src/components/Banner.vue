<template>
    <div id="main-banner">
        <h1>Sorveteria Hero</h1>
    </div>
</template>

<script>
    export default{
        name: 'Banner'
    }
</script>

<style scoped>
    #main-banner {
        background-image: url('/images/banner.jpg');
        background-position: 0 -250px;
        background-size: 115%;
        height: 500px;
        display: flex;
        align-items: center;
        justify-content: flex-start;
    }

    #main-banner h1 {
        color: #DB4D89;
        text-align: center;
        font-size: 50px;
        background-color: #9FD9FF;
        padding: 20px 40px;
    }
</style>
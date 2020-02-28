<template>
    <div class="column col-xl-2 col-lg-2 col-md-3 col-sm-4 col-xs-6 p-2 my-2">
        <div class="container p-2 my-2">
            <span :class="`icon ${icon}`"></span>
            <span>{{text}}</span>
        </div>

    </div>
</template>

<script>
    export default {
        name: "Icon",
        props: ['icon', 'text']
    }
</script>

<style scoped>
    span {
        display: block;
        text-align: center;
    }

    .icon{
        font-size:2.5em;
    }
</style>
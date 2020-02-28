<template>
    <div class="container bg-gray p-2 mt-2 ">
        <h6 class="text-bold text-uppercase text-center mt-2 pt-2">{{ title}}</h6>
        <div class="columns p-2 m-2 ">
            <icon :link="link" v-for="link in links" :key="link.icon"/>
        </div>
    </div>
</template>

<script>
    import Icon from "./Icon";
    export default {
        name: "Links",
        components: {Icon},
        props: ['title', 'links'],

    }
</script>

<style scoped>

</style>
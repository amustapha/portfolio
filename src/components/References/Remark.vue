<template>
    <figure class="carousel-item bg-gray">
        <blockquote>
            <slot></slot>
        </blockquote>
        <h5 class="mb-0">{{ author }} </h5>
        <small>{{ about }}</small>
    </figure>
</template>

<script>
    export default {
        name: "Remark",
        props: [
            'author', 'about', 'next', 'prev'
        ]
    }
</script>

<style scoped>
    .btn-action {
        top: 0;
    }

</style>
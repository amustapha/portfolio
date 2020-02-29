<template>
    <div class="hero hero-lg bg-primary  px-2">
        <div class="hero-body text-center px-2 mx-2">
            <img src="my-pic-no-bg.png" class="me" height="460px" />
            <h1 class="text-bold front">Abdulhakeem Adetunji Mustapha</h1>
            <p class="my-about front">Creative and result-oriented Software Engineer with over 6 years of experience building amazing web and
                mobile applications, coordinating cross-functional teams and easily communicating complex technical
                details to non-technical stakeholders.</p>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Hero"
    }
</script>

<style scoped>
    .my-about {
        max-width: 680px;
        margin: auto;
    }

    .me {
        position: absolute;
        bottom: 0;
        left: 0;
        z-index: 1;
    }

    .front {
        z-index: 20;
    }

    .hero{
        position: relative;
    }

    @media (min-width: 1146px) {
        .hero-body {
            margin-left: 256px !important;
        }
    }

    @media (min-width: 800px) {
        .hero-body {
            margin-left: 400px !important;
        }
    }

    @media (max-width: 800px) {
        .hero-body img {
            display: none;
        }
    }

</style>
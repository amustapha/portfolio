<template>
    <div class="hero hero-lg bg-primary  px-2">
        <div class="hero-body text-center px-2 mx-2">
            <img src="my-pic-no-bg.webp" class="me" height="460px" alt="My picture"/>
            <h1 class="text-bold front">Abdulhakeem Adetunji Mustapha</h1>
            <p class="my-about front mb-2 pb-2" v-if="show == 1">Creative and result-oriented Software Engineer with
                over 6 years of
                experience building amazing web and
                mobile applications, coordinating cross-functional teams and easily communicating complex technical
                details to non-technical stakeholders.</p>
            <p class="my-about front mb-2 pb-2" v-else>
                I'm a backend developer who is not scared of the frontend. With over 6 years experience in
                building and deploying mobile and web applications, I've become a real jack of all trade, master of pun.<br/>
                Not to brag, I consider myself to be among the top 1% of the best 1%.
            </p>
            <a href="https://docs.google.com/document/d/1xElMvl-O5xN6oA5U989hwJlEwEseLTA-QxpNFkxs73Q/edit?usp=sharing"
               target="_blank"
               rel="noopener"
               class="btn mt-2 text-uppercase text-bold bg-dark btn-primary">Checkout my resume</a>

            <a href="mailto:abdulhakeemmustapha@gmail.com?subject=I've a Project for you&body=Hi Abdul,"
               class="btn mt-2 text-bold mx-2 text-uppercase" target="_blank" rel="noopener">
                Hire Me
            </a>
            <div class="lnks">
                <a href="https://blog.amustapha.com" class="text-light" rel="noopener">My Blog</a>
                <a href="mailto:abdulhakeemmustapha@gmail.com" class="text-light hide-md" rel="noopener">
                    abdulhakeemmustapha@gmail.com
                </a>
                <a href="tel:+2347067577058" class="text-light">+234 706 757 7058</a>
            </div>
        </div>

    </div>
</template>

<script>
    export default {
        name: "Hero",
        computed: {
            show: function () {
                let current = window.localStorage.getItem('current')
                if (current) {
                    current = parseInt(current)
                    current += 1
                    current %= 2
                } else {
                    current = Math.ceil(Math.random() * 2)
                }
                window.localStorage.setItem('current', current)
                return current
            }
        }
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

    .lnks {
        position: absolute;
        top: 0;
        right: 0;
        padding: 24px;
    }

    .lnks a {
        padding: 16px;
    }

    .front {
        z-index: 20;
    }

    .hero {
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
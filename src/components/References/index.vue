<template>
    <div class="container bg-gray p-2 mt-2">
        <div class="container container-fluid">
            <h6 class="text-bold text-uppercase text-center">Some people I've worked with</h6>
            <div class="carousel">
                <!-- carousel locator -->
                <input class="carousel-locator" id="slide-1" type="radio" name="carousel-radio" hidden="" checked="">
                <input class="carousel-locator" id="slide-2" type="radio" name="carousel-radio" hidden="">
                <input class="carousel-locator" id="slide-3" type="radio" name="carousel-radio" hidden="">
                <input class="carousel-locator" id="slide-4" type="radio" name="carousel-radio" hidden="">

                <!-- carousel container -->
                <div class="carousel-container">
                    <!-- carousel item -->
                    <remark author="Daniel Roy Greenfiled"
                            about="Vice President at BriteCore. Worked at NASA 2005-2010. Principal at Cartwheel Web since 2010. Co-authored the Two Scoops of Django books.">
                        Abdulhakeem was someone I hired to work under me at BriteCore. He is conscientious and
                        intelligent, able to solve hard problems but modest in his interactions with others. He has
                        a natural instinct for doing things the right way, yet understands that sometimes the needs
                        of business forces a quicker solution that can be optimized later.<br/>
                        In summary, if my new company were hiring I would bring him into my new team today.
                    </remark>

                    <remark author="Chukwudi Nwachukwu"
                            about="Software Architect | PSF Fellow | ex Python Nigeria Community Chairperson | PyCon Nigeria/Africa Co-organizer">
                        I have worked with Abdulhakeem and he is well positioned to handle dynamic jobs. Abdul, as I
                        fondly call him, never missed his deadlines. He is also versed in many areas of programming and
                        has demonstrated that several times.
                    </remark>
                    <remark author="Timothy Olaleke"
                            about="Software Engineer at Mercurie | DSC Mentor | Google Developer Expert, Cloud">
                        As a colleague, I have worked with Abdulhakeem Mustapha on projects where he showed an exception
                        ability to solve problems using the right tools. He also has great experience in building
                        customer centric applications at a large scale.
                    </remark>
                    <remark author="Peter Olayinka"
                            about="Software Engineer at Britecore">
                        Abdulhakeem is such a very detailed person, we both worked in the same team for months and he is
                        such a team player. I could remember days when the we will be required to some task done and the
                        whole team will stay up all night on a Video Call. Thank you so much for being such a team
                        player.
                    </remark>
                </div>
                <!-- carousel navigation -->
                <div class="carousel-nav">
                    <label class="nav-item text-hide c-hand text-dark" for="slide-1" ref="c-1">1</label>
                    <label class="nav-item text-hide text-dark c-hand" for="slide-2" ref="c-2">2</label>
                    <label class="nav-item text-hide text-dark c-hand" for="slide-3" ref="c-3">3</label>
                    <label class="nav-item text-hide text-dark c-hand" for="slide-4" ref="c-4">4</label>
                </div>
            </div>
        </div>
    </div>

</template>

<script>
    import Remark from "./Remark";

    export default {
        name: "References",
        components: {Remark},
        data () {
            return {
                active: 1
            }
        },
        mounted() {
            const context = this
            setInterval(function () {
                console.log(context.active)
                context.$refs[`c-${(++context.active % 4) + 1}`].click()
            }, 5000)
        }
    }
</script>

<style scoped>
    .container-fluid {
        max-width: 840px;
    }

    @media (min-width: 960px) {
        .carousel-container::before {
            padding-bottom: 256px !important;
        }
    }

    @media (min-width: 600px) {
        .carousel-container::before {
            padding-bottom: 340px;
        }
    }

    @media (max-width: 600px) {
        .carousel-container::before {
            padding-bottom: 380px;
        }
    }

</style>
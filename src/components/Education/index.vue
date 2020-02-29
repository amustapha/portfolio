<template>
    <div class="container container-fluid">
        <h2 class="text-bold text-uppercase text-center">Where I've studied</h2>
        <div class="timeline p-2">
            <single company="Bayero University" role="BS Computer Science"
                    dates="April, 2013 - January, 2017">
                <ul>
                    <li>
                        Recipient of "Most Innovative Student" Award.
                    </li>
                    <li>
                        Graduated with a 4.15 GPA.
                    </li>

                </ul>
            </single>
        </div>
    </div>

</template>

<script>
    import Single from "./Single";

    export default {
        name: "Education",
        components: {Single}
    }
</script>

<style scoped>

</style>
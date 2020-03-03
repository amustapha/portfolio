<template>
    <div class="container container-fluid">
        <h2 class="text-center text-uppercase text-bold">Some of my projects</h2>
        <div class="columns">
            <single-project
                    title="Lissafi"
                    link="https://app.lissafi.com"
                    summary="Accounting software for small & medium businesses"
                    :icons="['icon-django', 'icon-vue-dot-js', 'icon-amazonaws', 'icon-mysql', 'icon-node-dot-js', 'icon-flask']">
                <p>
                    Building an accounting software for small and medium scale businesses, including accessibility
                    features for people with little educational background.
                </p>
            </single-project>
            <single-project
                    title="Ji's Kitchen"
                    link="https://jiskitchen.com"
                    summary="On demand food delivery service"
                    :icons="['icon-django', 'icon-vue-dot-js', 'icon-googlecloud']">
                <p>
                    Developed and managed a simple food ordering site for the Bayero University community keeping time
                    to meaningful interaction very low.

                </p>
            </single-project>
            <single-project
                    title="Pipersoft"
                    link="https://piper.com.ng"
                    summary="Bookkeeping & Inventory management software"
                    :icons="['icon-django', 'icon-vue-dot-js', 'icon-googlecloud', 'icon-couchdb-icon', 'icon-pouchdb']">
                <p>
                    Architect, built and deployed an inventory management software for businesses. With accounting
                    and balances accessible in a few clicks.

                </p>
            </single-project>

            <single-project
                    title="Mosh Oyewole"
                    summary="Crowdfunding platform for election"
                    :icons="['icon-html5', 'icon-css3', 'icon-php', 'icon-bootstrap', 'icon-cpanel']">
                <p>
                    Gofund me and other cause crowdfunding platforms are not open for Nigerians, we developed a campaign
                    site including functionaliy for collecting donations.
                </p>
            </single-project>
            <single-project
                    title="Farmerinsuit"
                    link="https://farmerinsuit.com"
                    summary="Crowdfunding platform for agriculture"
                    :icons="['icon-django', 'icon-googlecloud', 'icon-bootstrap']">
                <p>
                    A crowd-funding platform for providing financing, technical support and agricultural extension
                    services for rural
                    farmers improving their yield and livelihood.
                </p>
            </single-project>
            <single-project
                    title="Cammart"
                    summary="Mini e-commerce for college campus"
                    :icons="['icon-php', 'icon-mysql', 'icon-java', 'icon-googleplay']">
                <p>
                    With difficulty associated with getting groceries on campus for university students, cammart
                    provided a mobile application for ordering groceries.
                </p>
            </single-project>

        </div>
        <div class="column">
            <span class=""> </span>
        </div>
        <div class="column">
            <span class=""> </span>
        </div>
        <div class="column">
            <i class=""> </i>
        </div>
        <div class="column">
            <i class=""> </i>
        </div>
    </div>


</template>

<script>
    import SingleProject from "./SingleProject";

    export default {
        name: "Projects",
        components: {SingleProject}
    }
</script>

<style scoped>

</style>
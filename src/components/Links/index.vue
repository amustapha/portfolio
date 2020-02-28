<template>
    <div class="container bg-gray p-2">
        <div class="columns p-2 m-2">
            <icon :icon="tech.icon" :text="tech.text" v-for="tech in techs" :key="tech.icon"/>

        </div>
    </div>
</template>

<script>
    import Icon from "./Icon";
    export default {
        name: "Links",
        components: {Icon},
        data () {
            return {
                techs: [
                    {
                        icon: 'icon-python',
                        text: 'Python'
                    },
                    {
                        icon: 'icon-django',
                        text: 'Django'
                    },
                    {
                        icon: 'icon-javascript',
                        text: 'Javascript'
                    },
                    {
                        icon: 'icon-flask',
                        text: 'Flask'
                    },
                    {
                        icon: 'icon-vue-dot-js',
                        text: 'Vue JS'
                    },
                    {
                        icon: 'icon-amazonaws',
                        text: 'AWS'
                    },
                    {
                        icon: 'icon-mongodb',
                        text: 'MongoDB'
                    },
                    {
                        icon: 'icon-googlecloud',
                        text: 'GCP'
                    },
                    {
                        icon: 'icon-java',
                        text: 'Java'
                    },
                    {
                        icon: 'icon-c',
                        text: 'C/C++'
                    },
                    {
                        icon: 'icon-docker',
                        text: 'Docker'
                    },
                    {
                        icon: 'icon-jira',
                        text: 'Jira'
                    }
                ]
            }
        }
    }
</script>

<style scoped>

</style>
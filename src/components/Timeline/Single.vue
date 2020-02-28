<template>
    <div class="timeline-item" id="timeline-example-2">
        <div class="timeline-left">
            <a :class="latest? '': 'timeline-icon icon-lg'" href="#timeline-example-2">
                <i :class="latest ? 'timeline-icon' :  'icon icon-checkmark'"></i>
            </a>
        </div>
        <div class="timeline-content">
            <h5 class="text-primary">{{role}} at {{ company }}  <small class="dates text-italic text-gray"> {{dates }} </small></h5>
            <slot></slot>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Single",
        props: ['latest', 'company', 'role', 'dates'],

    }
</script>

<style scoped>

    @media (min-width: 640px) {
        .dates {
            float: right;
        }
    }

    @media (max-width: 640px) {
        .dates {
            display: block;
        }
    }

</style>
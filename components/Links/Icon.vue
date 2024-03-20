<template>
  <div class="column col-xl-2 col-lg-2 col-md-3 col-sm-4 col-xs-6 p-2 my-2">
    <a :href="link.target" target="_blank" class="container p-2 my-2 external-link">
      <span :class="` icon ${link.icon} ${extra} `"></span>
      <span>{{ link.text }}</span>
    </a>
  </div>
</template>

<script>
export default {
  name: "Icon",
  props: {
    link: {
      type: Object,
      required: true,
    },
  },
  methods: {
    open(target = null) {
      if (target != null) {
        window.location.href = target;
      }
    },
  },
  computed: {
    extra() {
      return this.link.target ? "c-hand" : "";
    },
  },
};
</script>

<style scoped>
span {
  display: block;
  text-align: center;
}

.icon {
  font-size: 2.5em;
}

.external-link {
    text-decoration: none;
    color: inherit;
    cursor: pointer;
    transition: all 0.3s;
}
</style>

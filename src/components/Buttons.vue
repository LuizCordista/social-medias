<script>
export default {
  props: {
    label: {
      type: String,
      required: true
    },
    link: {
      type: String,
      required: true
    }
  }
}
</script>

<template>
<a :href="link" target="_blank">{{ label }}</a>
</template>

<style scoped>
a {
  display: block;
  color: var(--neutral-white);
  font-weight: 600;
  text-decoration: none;
  background-color: var(--neutral-grey);
  border-radius: 6px;
  width: 360px;
  margin: 0 auto 0 auto;
  padding:16px
}

a:hover {
  background-color: var(--primary-color);
  color: var(--neutral-darkgrey);
}

@media (max-width: 480px) {
  a {
    width: 100%;
  }
}

</style>
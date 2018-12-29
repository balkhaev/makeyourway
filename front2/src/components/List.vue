<template>
  <a-card :title="title" :bordered=false>
    <slot></slot>
  </a-card>
</template>

<script>
  export default {
    props: ['title'],
  }
</script>

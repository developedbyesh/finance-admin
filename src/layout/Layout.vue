<template>
  <b-container
    class="d-flex flex-column align-items-center justify-content-center mx-0 px-0 root-layout"
    fluid
  >
    <slot></slot>
  </b-container>
</template>
<style scoped>
.root-layout {
  position: relative;
  min-height: 100vh;
  width: 100%;
  top: 0;
  left: 0;
}
</style>
+
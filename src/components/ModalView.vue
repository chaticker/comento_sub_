<template>
  <div class="modal">
    <div class="overlay" @click="$emit('close-modal')"></div>
    <div class="modal-card">
      <slot />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
/* Modal */
.modal,
.overlay {
  width: 100%;
  height: 100%;
  position: fixed;
  left: 0;
  top: 0;
}
.overlay {
  opacity: 0.5;
  background-color: black;
}
.modal-card {
  position: relative;
  margin: auto;
  margin-top: 200px;
  width: 460px;
  height: 268px;
  padding: 15px 15px 30px 30px;
  background-color: white;
  z-index: 10;
  opacity: 1;
}
</style>
<template>
    <button id="btn-ir-arriba">
        <svg viewBox="0 0 24 24">
            <path d="m4 16 8-8 8 8"></path>
        </svg>
    </button>
</template>

<script>
export default {
      name: 'BotonArriba',
    }
document.addEventListener("DOMContentLoaded", () => {

const scrollToBottomButtom = document.getElementById('btn-ir-arriba');

window.addEventListener("scroll", () => {
  if (window.scrollY > 100) {
    scrollToBottomButtom.style.display = 'block';
  } else {
    scrollToBottomButtom.style.display = 'none';
  }
});

scrollToBottomButtom.addEventListener('click', () => {
  window.scrollTo({
    top: 0,
    // behavior: 'smooth'
  });
});

});

</script>

<style>

</style>
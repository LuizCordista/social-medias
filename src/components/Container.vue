<script setup>
import Button from "@/components/Buttons.vue";

</script>

<template>
<div class="container">
  <img src="@/assets/foto.jpeg" width="128px">
  <h2>Luiz Cordista</h2>
  <h3>Belo Horizonte, Minas Gerais</h3>
  <p>"Estudante de Engenharia de Software."</p>
  <div class="buttons">
    <Button label="GitHub" link="https://github.com/LuizCordista"></Button>
    <Button label="LinkedIn" link="https://www.linkedin.com/in/luizcordista/"></Button>

  </div>
</div>
</template>

<style scoped>

img {
  border-radius: 100%;
  margin: 0 auto 24px auto;
}

h2 {
  color: var(--neutral-white);
  font-weight: 600;
  margin-bottom: 8px;
  font-size: 1.5rem;
}

h3 {
  color: var(--primary-color);
  font-weight: 600;
  font-size: 1rem;
  margin-bottom: 24px;
}

p {
  color: var(--neutral-white);
  margin-bottom: 24px;
}

.container {
  padding: 48px;
  display: flex;
  flex-direction:column;
  border-radius: 12px;
  background-color:var(--neutral-darkgrey);
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.buttons {
  display: flex;
  flex-direction: column;
  gap: 12px;
}

@media (max-width: 480px) {
  .container {
    width: calc(100vw - 48px);
    padding: 48px 24px 48px 24px;
  }
}

</style>
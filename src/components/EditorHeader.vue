<template>
  <div class="header">
    <img src="/icon.png" alt="UniCucumber" class="logo" />
    <h1 class="title"><span style="color: #000">Uni</span>Cucumber</h1>
  </div>
  <div class="modal-buttons">
    <button @click="$emit('openSettings')" class="modal-button">
      <span class="material-symbols-outlined bold">settings</span>
    </button>
    <button @click="$emit('toggleSidebar')" class="modal-button">
      <span class="material-symbols-outlined bold">glyphs</span>
    </button>
    <a href="https://github.com/SkyEye-FAST/unicucumber" class="github-link">
      <img src="/github-icon.svg" alt="GitHub" class="github-icon" />
    </a>
  </div>
</template>

<script setup>
defineEmits(['openSettings', 'toggleSidebar'])
</script>

<style scoped>
.header {
  display: flex;
  align-items: center;
}

.logo {
  width: 2.5em;
  height: 2.5em;
  margin-right: 10px;
  margin-top: 20px;
}

.title {
  font-family: 'Noto Sans', sans-serif;
  font-size: 2em;
  color: var(--primary-color);
  margin-bottom: 5px;
}

.modal-buttons {
  display: flex;
  margin: 5px;
  align-items: center;
  flex-direction: row;
}

.modal-button {
  color: var(--primary-color);
  background-color: inherit;
  font-size: 1.5em;
  padding: 5px;
  margin: 0 10px;
  cursor: pointer;
  border: none;
  transition: color 0.3s ease;
}

.modal-button:hover {
  color: var(--primary-dark);
}

.github-link {
  transform: translateY(-0.1em);
}

.github-icon {
  width: 1.4em;
  padding: 5px;
  margin: 0 10px;
}

@media (orientation: portrait) and (min-width: 768px) and (max-width: 1024px) {
  .modal-button {
    padding: 5px 10px;
    font-size: 2em;
  }

  .github-icon {
    width: 2.1em;
    padding: 5px 10px;
  }

  .title {
    font-size: 3em;
  }

  .logo {
    width: 3.5em;
    height: 3.5em;
    margin-top: 30px;
  }
}

@media (orientation: portrait) and (min-width: 1024px) {
  .modal-button {
    font-size: 3em;
    padding: 10px 15px;
  }

  .github-icon {
    width: 3.2em;
    padding: 10px 15px;
  }

  .title {
    font-size: 4em;
  }

  .logo {
    width: 5em;
    height: 5em;
    margin-top: 40px;
  }
}
</style>

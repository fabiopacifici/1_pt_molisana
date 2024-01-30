<script>

import AppLogo from './AppLogo.vue';

export default {
  name: 'AppHeader',
  components: {
    AppLogo
  }
}
</script>
<template>
    <header>
      <AppLogo></AppLogo>
      <nav>
        <ul class="main_menu">
          <li><a href="#">Home</a></li>
          <li><a href="#" class="active">Prodotti</a></li>
          <li><a href="#">Chi siamo</a></li>
          <li><a href="#">Contatti</a></li>
        </ul>
      </nav>
    </header>
</template>


<style scoped>

header {
  background-color: var(--mol-light);
  text-align: center;
  padding: 2rem 0;

  & .main_menu {
    margin-top: 2rem;
    list-style: none;
    display: flex;
    justify-content: center;
  
    & a {
      text-decoration: none;
      padding: 1.5rem 1rem;
      color: var(--mol-dark);
      font-weight: 600;
    }

    & a.active {
      background-color: var(--mol-primary);
    }

  }

}

</style>
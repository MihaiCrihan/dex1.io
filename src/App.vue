<template>
  <v-app>
    <v-app-bar
      height="40"
      app
      elevate-on-scroll
      dark
    >
      <div class="d-flex align-center heading-5">n
        Сергей Лазарев
      </div>

      <v-spacer></v-spacer>
      <div class="menus d-flex">
        <div>
          <a href="#songs">
            Песни
          </a>
        </div>
        <div>
          <a href="#photo-galery">
            Фото Галерея
          </a>
        </div>
        <div>
          <a href="#about" >
            О певце
          </a>
        </div>
        <div>
          <a href="#eurovision">
            Проекты
          </a>
        </div>
      </div>
    </v-app-bar>

    <v-main>
      <HelloWorld/>
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld'

export default {
  name: 'App',

  components: {
    HelloWorld,
  },

  data: () => ({
    //
  }),
}
</script>
<style>
  ::-webkit-scrollbar {
    width: 6px;
  }

  /* Track */
  ::-webkit-scrollbar-track {
    box-shadow: inset 0 0 5px grey;
    border-radius: 10px;
  }

  /* Handle */
  ::-webkit-scrollbar-thumb {
    background: #4f4f4f;
    border-radius: 10px;
  }

  .menus >>> a {
    text-decoration: none;
    color: #FFFFFF;
    display: inline-block;
  }
  .menus div {
    margin: 0 8px;
  }

  .v-application a {
    color: #ffffff !important;
  }
  a:link {
    text-decoration: none;
  }

  a:visited {
    text-decoration: none;
  }

  a:hover {
    text-decoration: none;
  }

  a:active {
    text-decoration: none;
  }
</style>

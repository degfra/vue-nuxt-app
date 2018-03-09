<template>
  <header class="header">
      <ul class="nav-items">
          <li>
              <nuxt-link to="/">Home</nuxt-link>
          </li>
          <li>
              <nuxt-link to="/users">Users</nuxt-link>
          </li>
      </ul>
  </header>
</template>

<style scoped>
    .header {
        width: 100%;
        height: 60px;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: #ccc;
        font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
        font-size: 16px;
        word-spacing: 1px;
        -ms-text-size-adjust: 100%;
        -webkit-text-size-adjust: 100%;
        -moz-osx-font-smoothing: grayscale;
        -webkit-font-smoothing: antialiased;
    }

    .nav-items {
        list-style: none;
        padding: 0;
        margin: 0;
        display: flex;
        justify-content: space-around;
        align-items: center;
        width: 80%;
    }

    .nav-items a {
        text-decoration: none;
        color: black;
    }

    .nav-items a:hover,
    .nav-items a:active {
        color: white;
    }
</style>


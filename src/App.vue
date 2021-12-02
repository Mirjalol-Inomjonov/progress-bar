<template>
  <div id="app">
    <main>
      <div class="navigation">
        <header>
          <h1>Mirjalol Inomjonov</h1>
        </header>
        <nav>
          <ul>
            <li><router-link to="#">About me</router-link></li>
            <li><router-link to="#">Contact</router-link></li>
            <li><router-link to="#">Portfolio</router-link></li>
          </ul>
        </nav>
      </div>
      <Progressbar />
      <Post />
    </main>
    <router-view />
  </div>
</template>

<script>
import Post from "./components/Post";
import Progressbar from "./components/Progressbar";
export default {
  components: {
    Post,
    Progressbar,
  },
};
</script>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  text-decoration: none;
}
body {
  font-family: monospace, sans-serif;
}
main {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  overflow: hidden;
  // padding: 0 9%;

  .navigation {
    width: 100%;
    height: 10vh;
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: #000;
    padding: 30px 5%;
    header {
      h1 {
        font-size: 32px;
        color: #fff;
      }
    }
    nav {
      ul {
        list-style: none;
        li {
          display: inline-block;
          margin: 0 12px;
          a {
            margin: 0 20px;
            text-transform: uppercase;
            color: #fff;
          }
        }
      }
    }
  }
}
</style>

<template>
  <div id="app">
    <h1>Hallo!</h1>

    <p>Wij zijn de <a>Booze Brothers</a></p>
    <p>De leukste en gezelligste Amsterdamse cocktail catering van de wereld</p>
    <!-- <p></p> -->
    <p>Naast drank schenken drinken we het ook graag!</p>
    <div id="cta-button">
      <div class="inner">
        <font-awesome-icon :icon="['fas', 'comments']" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  margin-top: 60px;
}

body {
  font-family: "Rubik", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
    Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  font-size: calc(10px + 0.33vw);
  -webkit-font-smoothing: antialiased;
  padding: 5vh 10vw;
  /* color: #121314; */
  color: #fff;
  background-repeat: no-repeat;
  /* background-attachment: fixed;
  background-position: center; */
  background: url("assets/cocktail-2.jpg") no-repeat center center fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
}

h1 {
  font-size: 4.5em;
  font-weight: 600;
  margin-bottom: 0;
  color: #fff;
}

p {
  font-size: 1.6em;
  font-weight: 300;
  line-height: 1.4;
  max-width: 26em;
  color: #fff;
}

a {
  text-decoration: none;
  color: #fff;
  cursor: pointer;
  position: relative;
}

a:after {
  content: "";
  position: absolute;
  z-index: -1;
  top: 60%;
  left: -0.1em;
  right: -0.1em;
  bottom: 0;
  transition: top 200ms cubic-bezier(0, 0.8, 0.13, 1);
  background-color: rgba(204, 255, 204, 0.3);
}

a:hover:after {
  top: 0%;
}

#cta-button {
  position: absolute;
  background: #fff;
  color: red;
  height: 6em;
  width: 6em;
  border-radius: 3em;
  bottom: 1em;
  right: 1.5em;
}

.inner {
  position: relative;
  font-size: 3em;
  margin: 0 auto;
  width: 50%;
  height: 50%;
  -ms-transform: translateY(50%);
  transform: translateY(50%);
}
</style>

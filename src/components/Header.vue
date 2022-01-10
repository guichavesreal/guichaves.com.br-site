<template>
  <div class="header">
    <b-container fluid class="p-0 bg-dark">
      <div class="d-flex flex-row">
        <div class="d-inline-flex w-25 p-2">
          <h1 class="text-white p-2">{{ msg }}</h1>
        </div>
        <b-navbar class="d-inline-flex p-2 bd-highlight w-75 justify-content-end" type="dark" variant="dark">
          <b-navbar-nav>
            <b-nav-item href="#">Home</b-nav-item>
            <b-nav-item-dropdown text="Sobre" right>
              <b-dropdown-item href="#">Em breve</b-dropdown-item>
            </b-nav-item-dropdown>

            <b-nav-item-dropdown text="Contato" right>
              <b-dropdown-item href="#">Em breve</b-dropdown-item>
            </b-nav-item-dropdown>
          </b-navbar-nav>
        </b-navbar>
      </div>
    
    </b-container>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  font-family: 'Rock Salt', cursive;
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>

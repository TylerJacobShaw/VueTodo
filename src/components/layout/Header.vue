<template>
  <div>
    <header class="header">
      <h1 class="todoHeader">Todo List</h1>
      <div id="nav">
        <router-link class="link" to="/">Home</router-link>
        <!---->
        |
        <router-link class="link" to="/about">About</router-link>
      </div>
    </header>
  </div>
</template>
<script>
export default {
  name: "Header"
};
</script>
<style scoped>
.todoHeader {
  padding: 30px;
  text-align: center;
  background: black;
  color: white;
  font-size: 30px;
  margin: 0px;
}
#nav {
  text-align: center;
}
.link {
  text-decoration-color: cadetblue;
  text-decoration: none;
}
</style>



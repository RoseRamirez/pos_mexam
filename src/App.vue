<template>
  <div id="app">
    <div id="nav">
      <ul>
      <li><router-link to="/home">Home</router-link> </li>
      <li><router-link to="/about">About</router-link> </li>
      <li><router-link to="/databinding">Data Binding</router-link> </li>
      <li style="float:right"> <router-link to="/login">Login</router-link></li>
      </ul>

    </div>
    <router-view/>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

ul {
list-style-type: none;
margin: 0;
padding:0;
overflow: hidden;
background-color: rgb(255, 255, 255);
width: 100%;
}
li {
float: left;
}
li a {
display: block;
font-family:Verdana, Geneva, Tahoma, sans-serif;
font-size:20px;
font-weight: bolder;
color: rgb(5, 5, 5);
text-align: center;
padding: 14px 16px;
text-decoration: none;
}
li a:hover:not(.active) {
background-color: rgba(171, 173, 170, 0.986);
}
.active {
background-color: #4CAF50;
}
</style>

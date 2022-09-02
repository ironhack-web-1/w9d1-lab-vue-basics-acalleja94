<template>
  <div id="app">
  <h1>This is my form</h1>
    <form action="/form-result.php" method="post" target="_blank">

<input type="text" placeholder="Name" name="name" v-model="fName" />

<input type="email" placeholder="E-mail" name="email" v-model="fEmail" />

<button id="btn-form" type="submit">Submit</button>

</form>

<div id="binding">
  <h2>This is the two-day-data-binding result</h2>

<div class="form-res"><p>Your name is: {{fName}}</p></div>
<div class="form-res"><p>Your e-mail is: {{fEmail}}</p></div>
</div>

  </div>
</template>

<script>

export default {
  name: "App",
  data () {
    return {
      fName: '',
      fEmail: ''
    }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@400;600&display=swap');

#app {
  font-family: 'IBM Plex Mono', monospace;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-content: center;
  flex-direction: column;
}

form{
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 20px;
}

input{
  width: 200px;
  padding: 10px 2%;
  border: 1px solid #ccc;
  border-radius: 27px;
  height: 30px;
  font-family: 'IBM Plex Mono', monospace;
  font-size: 16px;
}

#btn-form{
  background:#000;
  color:#fafafa;
  height: 50px;
  width: 250px;
  border-radius: 27px;
  font-family: 'IBM Plex Mono', monospace;
  font-size: 16px;
}

#binding{
  width: 50%;
  margin: 50px auto;
  background: #6b61ab;
  padding: 50px;
  text-align: left;
}

#binding h2{
  color: #fafafa;
}

.form-res{
  background: #fafafa;
  width: 100%;
  text-align: left;
  color: rgb(72, 72, 72);
  padding: 1px;
  margin-top: 7px;
}

.form-res p{
  padding: 0 30px;
}

</style>

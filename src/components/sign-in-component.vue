<template>
<div class="box">
  <h1>Iniciar</h1>
 
  <div class="in">
      <label for="name">Mail</label>
    
      <div>  <input type="text" v-model="username" placeholder="E-mail"
           /><img v-if="username.length >= 4" src="../assets/ok.svg" alt=""></div>

  <div class="button_action">
    <button v-on:click="username = ' @gmail.com' ">@gmail.com</button> <button v-on:click="username = '@yahoo.com' ">@yahoo.com</button>  <button v-on:click="username = '@outlook.com' ">@outlook.com</button>  <button v-on:click="username = '@aol.com' ">@aol.com</button>
  </div>
  </div>

  <div class="in">
  <label for="name">Password</label>
  <div>
      <input v-model="password" type="password" :name="string" placeholder="Entrer votre mot de passe" required/><img v-if="password.length >= 8" src="../assets/ok.svg" alt="">
  </div>

  </div>

 
 
  <div class="check_bar">
    <div> <input type="checkbox" name="" id="">
    <label for="">Recordar</label></div>
  </div>


  <button class="log">
    Iniciar Sesión
    </button>
   

<span>No tienes cuenta? <a href="/signup">Registrate</a> </span> 
</div>

</template>


<script>
export default {

  data() {
    return {
      password:"",
      userLoggedIn: false,
      username:"",    
      isActive: false,
    };
    
  },toggle() {
this.isActive = ! this.enable ;
},
};

</script>





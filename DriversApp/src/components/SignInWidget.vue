<script>

export default {
  
}


</script>

<template>
  

  <div class="backPlate">
    
    <h1 class="title"> Sign In </h1>

    <div class="signIn">
    <p>Username</p>
    <input/>
    <p>Password</p>
    <input/>
    </div>

    <p class="link"><a src="#"> Forgot your Password? </a></p>
  </div>
  
</template>

<style>

input {
  height: 40px;
  width: 60%;
}

.backPlate {
  background-color: white;
  
  
}

.title {
  text-align: center;
}

.link {
  text-align: center;
}

.signIn {
  display: flex;
  flex-direction: column;
  gap: 30px;
  margin-bottom: 10%;
  
  
}

</style>

<template>
  <container class="cont" style="background-color:red">
    <headerLogin/>
    <div class="principal">
      <div class="base">
        <h1>Login</h1>
        <input type="text" name="usuario" value="Usuario" class="inputs" id="input1">
        <input type="password" name="senha" value="Senha" class="inputs" id="input2">
        <button> Enviar </button>
      </div>
    </div>
    <footers/>
  </container>
</template>

<script>

export default {
  name: 'home',
}

</script>

<style lang="scss" scoped>
@import "@/layouts/variaveis.scss"; 

.cont{
  height: $conte;
 
}

.principal{
  background-color: #E5E5E5;
  position: absolute;
  top: $alturaHeader;
  bottom: $alturaFooter;
  background-color: #E5E5E5;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

.base{
  background-color: #fff;
  width: 40%;
  height: 60%;
  padding: 3%;
  align-items: center;
  border-radius: 3px;
}

h1{
  font-weight: bold;
  text-align: center;
}

.inputs{
  padding: 0.7em 0.7em;
  border-radius: 6px;
  display: flex;
  flex-direction: column;  
  border-color: #ececec;
  align-items: center;
}

#input1{
  margin-top:10%;
}

#input2{
  margin-top:5%;
}

button {
 background: #D00000;
 padding: 0.5em 0.5em;
 border: none;
 border-radius: 7px;
 font-size: 17px;
 color: white;
 transition: all .5s ease-in-out;
 margin-top: 10%;
}

button:hover {
 animation: gradient 3s infinite;
 transform: scale(1.05);
}

</style>
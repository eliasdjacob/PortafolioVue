<script setup>

</script>

<template>
  <div class="wrapper">
    <form class="form">
      <div class="pageTitle title">Contacto</div>
      <div class="secondaryTitle title">Completá el formulario para contactarte.</div>
      <input type="text" class="name formEntry" placeholder="Nombre" />
      <input type="text" class="email formEntry" placeholder="Email" />
      <textarea class="message formEntry" placeholder="Mensaje"></textarea>
      <input type="checkbox" class="termsConditions" value="Term" />
      <label style="color: grey" for="terms">
        Acepto los <span style="color: #0e3721">términos</span> & <span style="color: #0e3721">condiciones</span>.
      </label>
      <br />
      <button type="submit" class="submit formEntry">Enviar</button>
    </form>
  </div>
</template>

<style scoped>
*, *:before, *:after {
  box-sizing: border-box;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

body {
  background: linear-gradient(to right, #ea1d6f 0%, #eb466b 100%);
  font-size: 12px;
  font-family: 'Brush Script MT', cursive;
}

body, button, input {
  font-family: 'Brush Script MT', cursive;
  font-weight: 700;
  letter-spacing: 1.4px;
}

.background {
  display: flex;
  min-height: 100vh;
}

.container {
  flex: 0 1 700px;
  margin: auto;
  padding: 10px;
}

.screen {
  position: relative;
  background: #3e3e3e;
  border-radius: 15px;
}

.screen:after {
  content: '';
  display: block;
  position: absolute;
  top: 0;
  left: 20px;
  right: 20px;
  bottom: 0;
  border-radius: 15px;
  box-shadow: 0 20px 40px rgba(0, 0, 0, .4);
  z-index: -1;
}

.screen-header {
  display: flex;
  align-items: center;
  padding: 10px 20px;
  background: #4d4d4f;
  border-top-left-radius: 15px;
  border-top-right-radius: 15px;
}

.screen-header-left {
  margin-right: auto;
}

.screen-header-button {
  display: inline-block;
  width: 8px;
  height: 8px;
  margin-right: 3px;
  border-radius: 8px;
  background: white;
}

.screen-header-button.close {
  background: #ed1c6f;
}

.screen-header-button.maximize {
  background: #e8e925;
}

.screen-header-button.minimize {
  background: #74c54f;
}

.screen-header-right {
  display: flex;
}

.screen-header-ellipsis {
  width: 3px;
  height: 3px;
  margin-left: 2px;
  border-radius: 8px;
  background: #999;
}

.screen-body {
  display: flex;
}

.screen-body-item {
  flex: 1;
  padding: 50px;
}

.screen-body-item.left {
  display: flex;
  flex-direction: column;
}

.app-title {
  display: flex;
  flex-direction: column;
  position: relative;
  color: #d5006d;
  font-size: 26px;
  font-family: 'Brush Script MT', cursive;
}

.app-title:after {
  content: '';
  display: block;
  position: absolute;
  left: 0;
  bottom: -10px;
  width: 25px;
  height: 4px;
  background: #d5006d;
}

.app-contact {
  margin-top: auto;
  font-size: 12px;
  color: #888;
  font-family: 'Brush Script MT', cursive;
}

.app-form-group {
  margin-bottom: 15px;
}

.app-form-group.message {
  margin-top: 40px;
}

.app-form-group.buttons {
  margin-bottom: 0;
  text-align: right;
}

.app-form-control {
  width: 100%;
  padding: 10px 0;
  background: none;
  border: none;
  border-bottom: 1px solid #666;
  color: #ddd;
  font-size: 14px;
  text-transform: uppercase;
  outline: none;
  transition: border-color .2s;
  font-family: 'Brush Script MT', cursive;
}

.app-form-control::placeholder {
  color: #666;
}

.app-form-control:focus {
  border-bottom-color: #ddd;
}

.app-form-button {
  background: none;
  border: none;
  color: #ffffff;
  font-size: 14px;
  cursor: pointer;
  outline: none;
  font-family: 'Brush Script MT', cursive;
}

.app-form-button.cancel {
  background-color: #d5006d;
}

.app-form-button.cancel:hover {
  background-color: #d5006d; 
  color: #ffffff; 
}

.app-form-button.send {
  background-color: #d5006d; 
}

.app-form-button.send:hover {
  background-color: #d5006d; 
  color: #ffffff; 
}

.app-form-button:hover {
  color: #b9134f; 
}

.credits {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 20px;
  color: #ffa4bd;
  font-family: 'Brush Script MT', cursive;
  font-size: 16px;
  font-weight: normal;
}

.credits-link {
  display: flex;
  align-items: center;
  color: #fff;
  font-weight: bold;
  text-decoration: none;
  font-family: 'Brush Script MT', cursive;
}

.dribbble {
  width: 20px;
  height: 20px;
  margin: 0 5px;
}

@media screen and (max-width: 520px) {
  .screen-body {
    flex-direction: column;
  }

  .screen-body-item.left {
    margin-bottom: 30px;
  }

  .app-title {
    flex-direction: row;
  }

  .app-title span {
    margin-right: 12px;
  }

  .app-title:after {
    display: none;
  }
}

@media screen and (max-width: 600px) {
  .screen-body {
    padding: 40px;
  }

  .screen-body-item {
    padding: 0;
  }
}

body {
  background-color: #d1f3e7;
}

.form {
  background: #fff;
  box-shadow: 0 30px 60px 0 rgba(90, 116, 148, 0.4);
  border-radius: 5px;
  max-width: 480px;
  margin: auto;
  padding-top: 5px;
  padding-bottom: 5px;
  position: relative;
  border-top: 5px solid #0e3721;
  animation: bounce 1.5s infinite;
  font-family: 'Brush Script MT', cursive;
}

::-webkit-input-placeholder {
  font-size: 1.3em;
  font-family: 'Brush Script MT', cursive;
}

.title {
  display: block;
  font-family: 'Brush Script MT', cursive;
  margin: 10px auto 5px;
  width: 300px;
}

.termsConditions {
  margin: 0 auto 5px 80px;
}

.pageTitle {
  font-size: 2em;
  font-weight: bold;
  font-family: 'Brush Script MT', cursive;
}

.secondaryTitle {
  color: grey;
  font-family: 'Brush Script MT', cursive;
}

.name {
  background-color: #ebebeb;
  color: white;
  font-family: 'Brush Script MT', cursive;
}

.name:hover {
  border-bottom: 5px solid #0e3721;
  height: 30px;
  width: 380px;
  transition: ease 0.5s;
}

.email {
  background-color: #ebebeb;
  height: 2em;
  font-family: 'Brush Script MT', cursive;
}

.email:hover {
  border-bottom: 5px solid #0e3721;
  height: 30px;
  width: 380px;
  transition: ease 0.5s;
}

.message {
  background-color: #ebebeb;
  overflow: hidden;
  height: 10rem;
  font-family: 'Brush Script MT', cursive;
}

.message:hover {
  border-bottom: 5px solid #0e3721;
  height: 12em;
  width: 380px;
  transition: ease 0.5s;
}

.formEntry {
  display: block;
  margin: 30px auto;
  min-width: 300px;
  padding: 10px;
  border-radius: 2px;
  border: none;
  transition: all 0.5s ease 0s;
  font-family: 'Brush Script MT', cursive;
}

.submit {
  width: 200px;
  color: white;
  background-color: #0e3721;
  font-size: 20px;
  font-family: 'Brush Script MT', cursive;
}

.submit:hover {
  box-shadow: 15px 15px 15px 5px rgba(78, 72, 77, 0.219);
  transform: translateY(-3px);
  width: 300px;
  border-top: 5px solid #0e3750;
  border-radius: 0%;
}

@keyframes bounce {
  0% {
    transform: translateY(10px);
  }
  50% {
    transform: translateY(-10px);
  }
  100% {
    transform: translateY(10px);
  }
}
</style>

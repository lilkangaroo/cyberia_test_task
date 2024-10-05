<template>
  <h2>Расскажите о вашем проекте:</h2>
  <form>
    <label for="userName">Ваше имя*</label>
    <input id="userName" type="text" maxLength="{50}" required />
    <label for="userEmail">Email*</label>
    <input id="userEmail" type="email" maxLength="{50}" required />
    <label for="telNo">Телефон*</label>
    <input id="telNo" type="tel" maxLength="{12}" required />
    <label for="userMessage">Сообщение*</label>
    <input id="userMessage" type="text" maxLength="{250}" required />
    <label for="userApproval">Согласие на обработку персональных данных</label>
    <input id="userApproval" type="checkbox" required />
    <button type="submit" name="send">Обсудить проект</button>
  </form>
</template>
<script></script>
<style></style>

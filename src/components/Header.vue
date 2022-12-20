<template>
  <header id="header">
    <a href=".">
      <img
        src="https://app.terappin.com/assets/logo-purple.3176330c.png"
        alt="terappin-logo"
      />
    </a>
    <button class="btn btn-primary">Testi Atla</button>
  </header>
</template>

<script>
export default {
  name: "header",
  data() {
    return {};
  }
};
</script>

<style>
#header {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  height: 100px;
  width: 90%;
  margin: auto;
}
#header a img {
  height: 50px;
}
</style>

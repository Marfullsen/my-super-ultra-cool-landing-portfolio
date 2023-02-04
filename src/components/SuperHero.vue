<template>
  <div>
    <aside p="x-4 y-10">
      super window
    </aside>
    Super Hero!
  </div>
</template>

<style scoped>
aside {
  width: 600px;
  height: 400px;
  border: 5px solid #a5cacf54;
  margin-left: auto;
  margin-right: auto;
  border-radius: 0.5em;
  background: radial-gradient(10px circle at 570px 10px, #b3cfd5 50%, transparent 50%)
    , radial-gradient(10px circle at 550px 10px, #b3cfd5 50%, transparent 50%)
    , radial-gradient(10px circle at 530px 10px, #b3cfd5 50%, transparent 50%);
    /* , linear-gradient(#b3cfd5 1.5em, #a5cacf54 1.5em, transparent 1.5em); */
  border: 9px solid lightskyblue;
  filter: drop-shadow(13px 12px 3px gray);
  background-color: #f4363600;
  /* width: 100px; */
  padding: 50px;
}
</style>

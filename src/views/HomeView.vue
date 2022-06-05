<template>
  <div class="home">
    <div class="box_name">
      <h1>Pet</h1>
      <div class="box_experience">
        <h1>Level: 2</h1>
        <h1>Next: 500xp</h1>
      </div>
    </div>
    <div id="porcentaje">
      <div class="barra_progreso">
        <span class="progreso" id="progreso"></span>
      </div>
    </div>
    <img class="box_pet" src="https://i.gifer.com/3IsJ.gif" alt="pet_default" />
  </div>
</template>

<script>
export default {
  name: 'HomeView',
}
</script>

<style lang="scss" scoped>
.home {
  margin: auto;
  text-align: center;
  top: 50%;
  left: 50%;
}

.box_name {
  text-align: left;
}

.box_pet {
  // position: absolute;
  width: 250px;
  height: 250px;
}

.barra_progreso {
  margin: auto;
  height: 40px;
  width: 50%;
  box-shadow: inset 6px 6px 12px #303030, inset -6px -6px 12px #404040;
  background-color: #383838;
  overflow: hidden;
  border-radius: var(--border_r);
}

.progreso {
  height: 100%;
  width: 0%;
  background-color: #15699e;
  box-shadow: 0 0 10px #15699e, 0 0 20px #15699e;
  display: block;
  border-radius: var(--border_r);
}

#porcentaje {
  font-size: 2.5px;
  font-family: sans-serif;
  font-weight: bold;
  text-align: center;
  transform: translateY(100px);
  color: #15699e;
}
</style>

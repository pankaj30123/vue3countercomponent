<template>
  <div class="text-center">
    <div id="compo">counter component</div>

    <div>
      <button id="colorb" @click.prevent="decreasecounter()">-</button>
      <span>{{ counter }}</span>
      <button id="colora" @click.prevent="increasecounter()">+</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      counter: 0,
    };
  },
  methods: {
    increasecounter() {
      this.counter++;
    },
    decreasecounter() {
      this.counter--;
    },
  },
};
</script>

<style>
#compo {
  font-size: 200%;
}
.text-center {
  text-align: center;
  color: red;
}
#colora,
#colorb {
  color: blue;
  height: 50px;
  width: 50px;
}
</style>

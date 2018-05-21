<template>
<<<<<<< HEAD
   <!-- インジケータ類 -->
   <div class="whackmole">
      <div class= "logo">モグラたたき！</div>
      <button class="game-start" v-on:click="gameStart">ゲーム開始</button>
      <div class=counter-container>
         <div class="counter">
            <h1>whacks:</h1>
            <h2>{{ score }}</h2>
         </div>
         <div class="counter">
            <h1>得点</h1>
            <h2>{{ highScore }}</h2>
         </div>
         <div class="counter">
            <h1>残り時間</h1>
            <h2>{{ timer }}</h2>
         </div>
      </div>
      <!-- モグラ表示 -->
      <div class="mole-container">
            <div class="mole">{{ moles[0] }}</div>
            <div class="mole">{{ moles[1] }}</div>
            <div class="mole">{{ moles[2] }}</div>
            <div class="mole">{{ moles[3] }}</div>
      </div>
   </div>
=======
  <div class="whackamole">
    <h1 class="logo">
      Whackamole
    </h1>
    <button 
      class="start-game"
      v-on:click="gameStart"
    >
      Start Game
    </button>
    <div class="counters-container">
      <div class="counter">
        <h1>Score:</h1>
        <h2>{{ score }}</h2>
      </div>
      <div class="counter">
        <h1>High Score:</h1>
        <h2>{{ highScore }}</h2>
      </div>
      <div class="counter">
        <h1>Timer:</h1>
        <h2>{{ timer }}</h2>
      </div>
    </div>
    <div class="moles-container">
      <div class="mole">{{ moles[0] }}</div>
      <div class="mole">{{ moles[1] }}</div>
      <div class="mole">{{ moles[2] }}</div>
      <div class="mole">{{ moles[3] }}</div>
    </div>
  </div>
>>>>>>> cb2ffb57bbfaf5392a613817d8d79f0b6f0e522e
</template>

<script>
export default {
<<<<<<< HEAD
   data: () => {
      return {
         score: 0,
         highScore: 15,
         timer: 20,
         moles: [false, false, false, false]
      };
   },
   methods: {
      gameStart: () => {
         alert('hello world');
      }
   }
=======
  name: 'App',
  data: () => {
    return {
      score: 0,
      highScore: 10,
      timer: 20,
      moles: [false, false, false, false]
    };
  },
  methods: {
    gameStart: function() {
      console.log('I was clicked!');
    }
  }
>>>>>>> cb2ffb57bbfaf5392a613817d8d79f0b6f0e522e
}
</script>

<style>
<<<<<<< HEAD
   .couter{
      margin: 10px;
      display: inline-block;
   }
   .mole{
      margin: 10px;
      display: inline-block;
   }
=======
.counter {
  margin: 10px;
  display: inline-block;
}

.mole {
  margin: 10px;
  display: inline-block;
}
>>>>>>> cb2ffb57bbfaf5392a613817d8d79f0b6f0e522e
</style>

<template>
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
    <Moles v-bind:moleData="moles"/>
  </div>
</template>

<script>
import Moles from './components/Moles';

export default {
  name: 'App',
  components: {'Moles': Moles},
  data: () => { //お作法 コンポーネントにデータを渡すときは関数にしてreturnしないといけない
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
}
</script>

<style>
   .couter{
      margin: 10px;
      display: inline-block;
   }
   .mole{
      margin: 10px;
      display: inline-block;
   }
</style>

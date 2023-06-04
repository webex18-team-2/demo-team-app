<template>
  <h1>Vue クイズ</h1>
  <div class="app">
    <h2>Q. 大三元.inc-名前由来</h2>
    <img
      class="quiz-image"
      src="https://img.ponparemall.net/imgmgr/37/00104837/kanji/tkanjiold_01/daisangen-tate.jpg?ver=1&size=pict650_650"
      alt="クイズタイトル"
    />
    <div class="container">
      <button v-on:click="answer1">中国の食べ物</button>
      <button v-on:click="answer2">麻雀</button>
      <button v-on:click="answer3">chatGPT命名</button>
    </div>
    <div>{{ answer }}</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      answer: "答えは...",
    }
  },
  methods: {
    answer1() {
      this.answer = "残念!!"
    },
    answer2() {
      this.answer = "正解!!"
    },
    answer3() {
      this.answer = "残念!!"
    },
  },
}
</script>

<style>
.app {
  display: flex;
  width: 100%;
  flex-direction: column;
  align-items: center;
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}

.quiz-image {
  height: 300px;
  width: 300px;
  object-fit: contain;
}

.container {
  display: flex;
  height: 2em;
  width: 300px;
  padding: 1em;
  justify-content: space-around;
}
</style>

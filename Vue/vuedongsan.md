```
<template>
  <div class="black-bg" v-if="모달창열렸니 == true">
    <div class="white-bg">
      <h4>상세페이지임</h4>
      <p>상세페이지 내용임</p>
      <button @click="모달창열렸니 = false">닫기</button>
    </div>
  </div>
  <div class="menu">
    <a v-for="a in menu" :key="a">{{ a }}</a>
  </div>
  <div>
    <h4 @click="모달창열렸니 = true">{{ products[0] }}</h4>
    <p>50만원</p>
    <button @click="신고수[0]++">허위매물신고</button>
    <span>신고수: {{ 신고수[0] }}</span>
  </div>
  <div>
    <h4>{{ products[1] }}</h4>
    <p>60만원</p>
    <button @click="신고수[1]++">허위매물신고</button>
    <span>신고수: {{ 신고수[1] }}</span>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      모달창열렸니: false,
      신고수: [0, 0],
      menu: ["Home", "Shop", "About"],
      products: ["역삼동원룸", "천호동원룸"],
    };
  },
  components: {},
};
</script>

<style>
body {
  margin: 0;
}

div {
  box-sizing: border-box;
}

.black-bg {
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.5);
  position: fixed;
  padding: 20px;
}

.white-bg {
  width: 100%;
  background: white;
  border-radius: 8px;
  padding: 20px;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.menu {
  background-color: darkslateblue;
  padding: 15px;
  border-radius: 5px;
}

.menu {
  color: white;
  padding: 10px;
}

.menu a {
  color: white;
  padding: 10px;
}
</style>

```

<script setup>
import Header from './components/Header.vue';
import ContentBoard from './components/ContentBoard.vue'
</script>

<template>
  <main>
    <ContentBoard class="main-bg">
      <div class="main-content">
        <Header />
      <div class="top">
        <div class="content">
          <div class="title">Gorgeous Code Snippets</div>
          <div>
            With Snipper, create fully customizable code snippets in a matter of seconds right from your browser.
          </div>
          <div>
            <button>Get started <span>- it's free</span></button>
          </div>
          <div>
            No credit card required.
          </div>
        </div>
      </div>
      <!-- 代码图片 -->
      <img class="top-img" src="@/assets/SnippetImage.png" alt="" />
      </div>
    </ContentBoard>
    <ContentBoard>
      <div class="c-detail">
        <div class="left">
          <div class="title">A fully customizable code snippet editor</div>
          <div>Fully customize the color scheme of your code snippet, or use our own premade color schemes. Export your
            code snippet in JPG, PDF, PNG, or any of the other 10+ common extensions.</div>
          <button>Get started <span>- it's free</span></button>
        </div>
        <div class="right">
          <img src="@/assets/CustomizableImage.png" alt="" />
        </div>
      </div>
      <div class="footer">
        <div>
          <img src="@/assets/Logo.svg" alt="" />
        </div>
        <div class="right">
          <span>Terms and Conditions</span>
          <span>Privacy Policy</span>
        </div>
      </div>
    </ContentBoard>
  </main>
</template>

<style>
body {
  font-size: 1.2rem;
  padding: 0;
  margin: 0;
}

.main-bg {
  background: top center / cover url('@/assets/Background.png') no-repeat;
}

.main-content {
  display: flex;
  flex-direction: column;
}

.top {
  display: flex;
  justify-content: center;
  text-align: center;
  font-size: 1.2rem;
  padding: 60px 0;
}

.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 20px;
  max-width: 600px;
}

.title {
  font-size: 3.7rem;
}

.top-img {
  width: 100%;
}

.c-detail {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap-reverse;
  gap: 50px;
  margin: 80px 0;
}

.c-detail .left {
  display: flex;
  flex-direction: column;
  gap: 20px;
  flex: 1;
  min-width: 380px;
  align-items: flex-start;
}

.c-detail .left .title {
  font-size: 2.8rem;
}

.c-detail .right img {
  width: 400px;
}

@media (max-width: 500px) {
  .c-detail .left {
    min-width: auto;
  }

  .c-detail .right {
    text-align: center;
  }
  .c-detail .right img {
    width: 90%;
    max-width: 400px;
  }
}

.footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100px;
  flex-wrap: wrap;
}
.footer .right {
  display: flex;
  gap: 20px;
  align-items: center;
}

button {
  background-color: black;
  color: white;
  padding: 15px 20px;
  border: 0;
  border-radius: 6px;
}
</style>

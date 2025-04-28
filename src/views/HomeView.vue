<script setup lang="ts">
import CallToActionButton from '@/components/CallToActionButton.vue'
</script>

<template>
  <main>
    <div class="left">
      <h1>Helping You Find Your Dream Home.</h1>
      <p>
        Derry Estate helps you find your dream home for your family, to be occupied or rented with
        trusted sources.
      </p>
      <CallToActionButton>
        <template #title>Find Home</template>
      </CallToActionButton>
    </div>
    <div class="right">
      <img src="@/assets/pictures/home.png" alt="" />
    </div>
  </main>
</template>

<style>
main {
  display: flex;
  justify-content: space-between;
  height: 100vh;
}
.left {
  width: 100%;
  background-image: url(/src/assets/pictures/home-bg-pattern.png);
  background-repeat: no-repeat;
  background-size: contain;
  display: flex;
  flex-direction: column;
  /* align-items: center; */
  justify-content: center;
  padding: 5vw;
}

.left h1 {
  color: #fff;
  font-weight: 800;
  font-size: 3.5em;
  line-height: 60px;
}

.left p {
  font-size: 1.3em;
  width: 80%;
  margin: 3vh 0;
  color: #fff;
}

.right {
  width: 100%;
  display: flex;
  justify-content: flex-end;
  align-items: flex-end;
}

.right img {
  width: 90%;
}
</style>

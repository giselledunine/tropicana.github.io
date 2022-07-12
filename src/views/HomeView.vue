<template>
  <div class="div">
    <div>
      <img
          alt="Vue logo"
          width="500"
          src="@/assets/logoLarge.png"
      />
    </div>
    <div>
      <img src="@/assets/button.png" alt="button">
    </div>
    <p class="cocktail">Cocktail challenge</p>
  </div>
  <div class="secondPart">
    <img src="@/assets/vage1.png" alt="vage1" class="width">
    <div class="sponsors">
      <h2>En compagnie de </h2>
      <div class="images">
        <img src="@/assets/darko.png" alt="darko" width="300">
        <img src="@/assets/champion.png" alt="champion" width="300">
      </div>
    </div>
    <img src="@/assets/vage2.png" alt="vague2" class="width">
  </div>
</template>

<style scoped>
.div {
  display: flex;
  align-items: center;
  flex-direction: column;
  width: 100vw;
  height: 90vh;
  background-image: url("@/assets/font.png");
  background-size: cover;
}
  .width {
    width: 100%;
  }
  .secondPart {
    margin-top: -105px;
  }

  .images {
    display: grid;
    grid-template-columns: 1fr 1fr;
    justify-items: center;
    width: 70%;
    margin: 0 auto;
  }

  .cocktail {
    font-size: 2rem;
    color: white;
    font-weight: bold;
  }

  h2 {
    color: white;
    text-align: center;
    font-weight: bold;
    margin-bottom: 2rem;
  }

  .sponsors {
    margin-top: -7px;
    background-color: #028343;
  }
</style>

<template>
  <main class="main">
    <h2 class="main__top">
        ❤️ dating site
      </h2>
      <h1 class="main__title">
        Meet 57k+ Girls in your city, right now!
      </h1>
    <div class="main__container container">
      <div class="main__inner">
          <img src="@/assets/girls/1.jpeg" alt="sexy girl" class="main__img">
        
          <img src="@/assets/girls/2.jpeg" alt="sexy girl" class="main__img">
        
          <img src="@/assets/girls/3.jpeg" alt="sexy girl" class="main__img">
        
          <img src="@/assets/girls/4.jpg" alt="sexy girl" class="main__img">
        
        <div class="main__circle circle">
          <h2 class="circle__title">
            Click to meet <br> local girls!
          </h2>
          <button class="circle__button">
            join now!
          </button>
        </div>
      </div>
    </div>
  </main>
</template>

<style lang="scss">
.main {
  display: flex;
  flex-direction: column;
  height: 100vh;
  &__container {
    display: flex;
    flex-direction: column;
  }
  &__top {
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 2rem;
    background-color: rgb(96, 47, 162);
    color: #fff;
    text-transform: uppercase;
    font-weight: 800;
    letter-spacing: 0.1rem;
  }
  &__title {
    text-align: center;
    color: #713fb2;
    padding: 1rem 0;
    font-weight: 700;
    font-size: 22px;  
  }
  &__inner {
    flex-grow: 1;
    position: relative;
    display: grid;
    width: 100%;
    height: 0;
    grid-template-rows: repeat(2, calc((100vh - 170px) / 2));
    grid-template-columns: repeat(2, 1fr);
    gap: 0.5rem 0.3rem;
  }
  & img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: 50% 0;
    border-radius: 2%;
  }
  &__circle {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
}

.circle {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: min(280px, 90%);
  aspect-ratio: 1/1;
  border-radius: 100%;
  background-color: rgba(233, 133, 120, 0.8);
  &__title {
    color: #fff;
    text-transform: uppercase;
    font-weight: 800;
    font-size: 24px;
    text-align: center;
    margin-bottom: 1rem;
  }
  &__button {
    background-color: rgb(235, 200, 70);
    color: #000;
    border-radius: 5%;
    border: none;
    padding: 0.5rem 2rem;
    font-weight: 800;
    font-size: 22px;
    cursor: pointer;
    transition: all 0.2s ease-in-out;
    box-shadow: 2px 2px 2px 2px #00000071;
    &:hover {
      transform: scale(1.05);
    }
  }
}
</style>
<template>
  <div class="mainPage">
   
    <div class="mainPage__background">
      <!-- <img src="../assets/background.jpg" alt="Background Image"> -->
    </div>
    <div class="mainPage__logo">  
      <img src="../assets/logo.png" alt="Logo">
    </div>
    <a href="https://calendly.com/jouennenicolas3" target="_blank" class="mainPage__button">
      <span>Réserver mon coaching</span>
    </a>
    <div class="mainPage__credits">
      <span>Anais Gourvest / </span>
      <span>Coach Sportif</span>
    </div>
  </div>
</template>

<script setup>

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
@import "../css/global.scss";

.mainPage {
        display: flex;
    justify-content: space-between;
    align-items: center;
    flex-direction: column;
    text-transform: uppercase;
    height: 100dvh;
    padding: 30px 0;
    box-sizing: border-box;
    overflow: hidden;

    &__background {
      position: absolute;
      top: 0;
      left: 0;
      background-image: url('../assets/background1.jpg'); /* mets le bon chemin */
      background-size: cover;        /* remplissage total */
      background-position: center;   /* centrer l’image */
      background-repeat: no-repeat;  /* ne pas répéter */
      object-fit: contain;
      min-height: 100vh;             /* au moins la hauteur de l’écran */
      width: 100vw;   
      z-index: -1; /* pour que le fond soit derrière les autres éléments */
    }

  &__logo {
    img {
      width: 120px;
      height: auto;
    }
  }
  
  &__button {
    width: 200px;
      height: 40px;
      background-color: rgba(0, 0, 0, 0.5); /* noir avec opacité 50% */
      
      border-radius: 25px; /* Bord arrondi */
      display: flex;
      justify-content: center;
      align-items: center;
      cursor: pointer;
      transition: background-color 0.3s ease;
      border: 2px solid $color-red;

    & span {
      color: #e3e3e3; /* Couleur du texte */
      font-family: $gotham-bold;
      font-size: 12px;
      font-weight: 400;
    }
      

      &:hover {
        background-color: rgba(0, 0, 0, 1);
      }
    
  }

  &__credits {
    color: $color-gray;
    font-size: 12px;
    letter-spacing: 3px;    

    & span:first-of-type {
      font-family: $gotham-black;
      font-weight: 300;
    }

    & span:last-of-type {
      font-family: $gotham-book;
      font-weight: 200;
    }
  }
}


</style>

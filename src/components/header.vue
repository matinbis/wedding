<script setup lang="ts">

</script>

<template>
 <img class="photo1" src="../assets/photo1.png" alt="">
 <div class="olive">
    <h1 class="title">Раз и навсегда.</h1>
    <h2 class="names">Соня и Данил</h2>
 </div>

 <div class="white">
    <h1 class="date">18.07.2026</h1>
    <p class="happy-text">Мы приглашаем вас разделить с нами радость рождения нашей семьи. Для нас это не просто праздник, а начало новой, красивой главы жизни, которую мы хотим открыть вместе с вами. Ждем вас с нетерпением, чтобы смеяться, танцевать и быть счастливыми в этот неповторимый день!</p>
</div>
<img class="photo2" src="../assets/photo2.png" alt="">
</template>

<style scoped>
.title, .names{
  font-family: "Playfair Display SC", serif;
  font-weight: 400;
  font-style: normal;
  font-size: 65px;
}

.date{
  font-family: "Smooch", cursive;
  font-weight: 400;
  font-style: normal;
  font-size: 80px;
}

.happy-text{
    font-size: 30px;
}

.olive{
    background: #A5BE94;
    color: white;
    min-height: 550px;
}
.white, .olive{
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}

.white{
    min-height: 550px;
}

.date, .happy-text{
    color: #927290;
    text-align: center;
    width: 800px;
}

.photo1, .photo2{
    position: absolute;
    width: 500px;
    opacity: 0;
}

.photo1{
    top: 70px;
    left: -600px;
    animation: slideLeft 1.5s ease forwards;
}

.photo2{
    top: 70px;
    right: -600px;
    animation: slideRight 1.5s ease forwards;
}

@keyframes slideLeft {
    to {
        left: 0;
        opacity: 1;
    }
}

@keyframes slideRight {
    to {
        right: 70px;
        opacity: 1;
    }
}

@media (max-width: 1920px){
    .photo1, .photo2{
        width: 400px;
    }
}

@media (max-width: 1350px){
    .photo1, .photo2{
        width: 300px;
    }
}

@media (max-width: 1080px){

    .olive{
        margin-top: 350px;
    }

  .title, .names{
    font-size: 36px;
  }

  .date{
    font-size: 50px;
  }

  .happy-text{
    font-size: 18px;
    width: 90%;
  }

  .white, .olive{
    min-height: auto;
    padding: 60px 20px;
  }

  /* Уменьшаем и позиционируем фото */
  .photo1, .photo2{
    width: 200px;
    position: absolute;
    top: 20px;
  }

  .date, .happy-text{
    max-width: 800px;
    width: 100%;
  }

  .photo1{
    left: -250px;
    animation: slideLeftMobile 1.2s ease forwards;
  }

  .photo2{
    right: -250px;
    animation: slideRightMobile 1.2s ease forwards;
  }

  @keyframes slideLeftMobile {
    to {
      left: -10px;
      opacity: 1;
    }
  }

  @keyframes slideRightMobile {
    to {
      right: 20px;
      opacity: 1;
    }
  }
}
</style>

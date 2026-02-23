<script setup lang="ts">

</script>

<template>
  <div class="background">
    <h1 class="title">План мероприятия</h1>
    <img src="../assets/when_photo1.png" class="when1" alt="">
    <div class="when">
        <div class="start">
            <h2>16:00</h2>
            <h3>Сбор гостей</h3>
        </div>
        <div class="end">
            <h2>23:00</h2>
            <h3>Окончание банкета</h3>
        </div>
    </div>
    <img src="../assets/when_photo2.png" class="when2" alt="">
 </div>
</template>

<style scoped>
    .background{
        position: relative;
        background: #ffffff;
        color: #D7B6A8;
        text-align: center;
        min-height: 1100px;
    }

    h1{
        font-family: "Playfair Display SC", serif;
        font-weight: 400;
        font-style: normal;
        font-size: 65px;
        padding-top: 200px;
    }

    .start, .end{
        padding: 50px;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
    }

    .when{
        padding-top: 50px;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: row;
        font-size: 50px;
    }

    h2{
        font-family: "Smooch", cursive;
        font-weight: 400;
    }

    h3{
        font-weight: 400;
    }

    .when1, .when2{
        position: absolute;
    }

    .when1{
        left: 20px;
        top: 360px;
    }

    .when2{
        right: 20px;
        top: 360px;
    }

@media (max-width: 768px) {
  .background {
    min-height: auto;
    padding: 40px 20px;
  }

  h1 {
    font-size: 40px;
    padding-top: 100px;
  }

  .when {
    flex-direction: row;
    justify-content: center;
    align-items: center;
    gap: 20px;
    font-size: 24px;
    padding-top: 30px;
  }

  .start, .end {
    padding: 20px;
  }

  .when1,
  .when2 {
    position: static;
    width: 290px; 
    height: auto;
  }

  .when1{
    display: none;
  }

  .background {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
}

@media (max-width: 1920px) {
    .when1, .when2{
        width: 400px;
        top: 550px;
    }
}

@media (max-width: 1220px){
    .when1, .when2{
        width: 350px;
        top: 660px;
    }
}
</style>

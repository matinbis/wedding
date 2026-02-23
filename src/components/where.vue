<script setup lang="ts">

</script>

<template>
 <div class="olive">
    <h1 class="title">Место проведения</h1>
    <div class="our_party">
        <div class="party1">
            <img src="../assets/med.png" alt="">
        </div>
        <div class="party2">
            <p>Наш праздник будет проходить в банкетном зале <strong>“Мёд”</strong> по адресу  улица 50-летия Магнитки, 58</p>
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2381.084279911328!2d58.95271597705008!3d53.35964657372784!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x43d12fed3f2d7275%3A0xd9109fb3ff536187!2z0JzQtdC0!5e0!3m2!1sru!2sru!4v1770740733051!5m2!1sru!2sru" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
    </div>
 </div>
</template>

<style scoped>
.olive{
    background: #A5BE94;
    color: white;
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    min-height: 1100px;
}

.title{
    font-family: "Playfair Display SC", serif;
    font-weight: 400;
    font-style: normal;
    font-size: 65px;
    padding-top: 50px;
}

.party1 img{
    border-radius: 6px;
    box-shadow: 10px 10px 10px #5a6851;
}

iframe{
    border-radius: 6px;
}

.our_party{
    margin-top: 30px;
    display: flex;
}

.party2{
    padding-top: 30px;
    max-width: 500px;
    margin-left: 50px;
}

iframe{
    margin-top: 30px;
}

p{
    font-size: 26px;
    text-align: left;
}

@media (max-width: 1200px) {

  .olive {
    min-height: auto;
    padding: 40px 20px;
  }

  .title {
    font-size: 40px;
  }

  .our_party {
    flex-direction: column;
    align-items: center;
  }

  .party1 img {
    width: 100%;
    max-width: 350px;
    height: auto;
  }

  .party2 {
    margin-left: 0;
    max-width: 100%;
    padding-top: 20px;
  }

  p {
    font-size: 18px;
    text-align: center;
  }

  iframe {
    width: 100%;
    height: 300px;
  }
}
</style>

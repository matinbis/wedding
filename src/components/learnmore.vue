<script setup lang="ts">
</script>

<template>
    <div class="pink">
        <h1 class="title">Остались вопросы?</h1>
        <div class="our_party">
            <div class="question-card">
                <div class="card-icon">📝</div>
                <p>Если вы планируйте посетить наш праздник, <b><i>обязательно</i></b> пройдите этот небольшой опрос</p>
                <a href="https://forms.gle/aS7psNN2qPZR5UWF8" class="link-card">
                    <span>Пройти опрос</span>
                    <span class="arrow">→</span>
                </a>
            </div>
            
            <div class="question-card">
                <div class="card-icon">💭</div>
                <p>Если у вас остались дополнительные вопросы, то мы рады будем ответить на них в беседе</p>
                <div class="social-links">
                    <a href="https://t.me/+nVi_ZMslWnM3OWQ6" class="social-link telegram">
                        <span>Телеграм</span>
                    </a>
                    <a href="https://vk.me/join/6wvnlOEuh3powAyWD0tF3GlPXCqIM2to7IU=" class="social-link vk">
                        <span>ВКонтакте</span>
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .pink{
        background: linear-gradient(135deg, #D7B6A8 0%, #c4a392 100%);
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

    .our_party{
        margin-top: 50px;
        display: flex;
        gap: 40px;
        max-width: 1200px;
        padding: 0 20px;
    }

    .question-card {
        flex: 1;
        background: rgba(255, 255, 255, 0.15);
        backdrop-filter: blur(10px);
        border-radius: 30px;
        padding: 40px;
        box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
        border: 1px solid rgba(255, 255, 255, 0.2);
        transition: all 0.3s ease;
    }

    .question-card:hover {
        background: rgba(255, 255, 255, 0.2);
        transform: translateY(-10px);
        box-shadow: 0 30px 50px rgba(0, 0, 0, 0.2);
    }

    .card-icon {
        font-size: 48px;
        margin-bottom: 20px;
    }

    p{
        font-size: 22px;
        text-align: left;
        margin-bottom: 30px;
        line-height: 1.6;
    }

    .link-card {
        display: inline-flex;
        align-items: center;
        gap: 10px;
        padding: 15px 30px;
        background: white;
        color: #D7B6A8;
        text-decoration: none;
        font-weight: 600;
        font-size: 18px;
        border-radius: 15px;
        transition: all 0.3s ease;
        box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
    }

    .link-card:hover {
        background: #D7B6A8;
        color: white;
        gap: 15px;
        box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
    }

    .arrow {
        font-size: 20px;
        transition: transform 0.3s ease;
    }

    .link-card:hover .arrow {
        transform: translateX(5px);
    }

    .social-links {
        display: flex;
        gap: 15px;
        justify-content: center;
    }

    .social-link {
        flex: 1;
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 10px;
        padding: 15px;
        border-radius: 15px;
        text-decoration: none;
        color: white;
        font-weight: 600;
        font-size: 18px;
        transition: all 0.3s ease;
        border: 2px solid transparent;
    }

    .social-link.telegram {
        background: #0088cc;
    }

    .social-link.vk {
        background: #4a76a8;
    }

    .social-link:hover {
        transform: scale(1.05);
        border-color: white;
    }

    @media (max-width: 768px) {
        .our_party {
            flex-direction: column;
        }
        
        .title {
            font-size: 36px;
        }
        
        p {
            font-size: 18px;
        }
        
        .social-links {
            flex-direction: column;
        }
    }
</style>
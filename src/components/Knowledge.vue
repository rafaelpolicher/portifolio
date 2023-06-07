<template>
    <section id="knowledge" v-motion-slide-visible-left>
        <h2>Knowledge</h2>
        <div class="knowledge-img">
            <div class="knowledge-group">
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-plain.svg" />
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-plain.svg" />
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-plain.svg" />
            </div>
            <div class="knowledge-group">  
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuejs/vuejs-original-wordmark.svg" />
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bootstrap/bootstrap-original-wordmark.svg" />
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original-wordmark.svg" />
            </div>
            <div class="knowledge-group">
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/php/php-plain.svg" />
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/laravel/laravel-plain-wordmark.svg" />
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original-wordmark.svg" />
            </div>
        </div>
    </section>
</template>
<style scoped>

h2{
    margin-bottom: 3rem;
}

.knowledge-group{    
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

img{
    width: 25vh;
    margin: 1rem 5rem;
    filter: grayscale(.9);
    position: relative;
    border-top: 4px solid #0F9410;
    border-bottom: 1px solid black;
    transition: .3s;

}

img:hover{
    filter: grayscale(0);
    border-top: 1px solid black;
    border-bottom: 4px solid #0F9410;
}

</style>
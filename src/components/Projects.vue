<template>
    <section id="projects" v-motion-slide-visible-left>
        <h2>Projects</h2>
        <div class="project-group">
            
            <div class="project">
                <a href="https://rafaelpolicher.github.io/dev-residencial/" target="_blank"><img class="main-img" src="../../public/img/dev.png" alt=""></a>
                <h3>Dev-Residencial</h3>
                <p>Fictional site for advertising land sales in a condominium</p>
                <ul>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-plain.svg" alt=""> HTML</li>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-plain.svg" alt=""> CSS</li>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-plain.svg" alt=""> JavaScript</li>
                </ul>
            </div>
            <div class="project">
                <a href="http://bookrating.x10.mx/" target="_blank"><img class="main-img" src="../../public/img/bookrating.png" alt=""></a>
                <h3>Bookrating</h3>
                <p>An book reviews website</p>
                <ul>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-plain.svg" alt=""> HTML</li>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-plain.svg" alt=""> CSS</li>
                    <li>Materialize CSS</li>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-plain.svg" alt=""> JavaScript</li>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/php/php-plain.svg" /> PHP </li>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/laravel/laravel-plain.svg" /> Laravel </li>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg" /> MySQL</li>
                </ul>
            </div>
            <div class="project">
                <a href="https://rafaelpolicher.github.io/costs/" target="_blank">
                <img class="main-img" src="../../public/img/costs.png" alt=""></a>
                <h3>Costs</h3>
                <p>A website to manage your project finances</p>
                <ul>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-plain.svg" alt=""> HTML</li>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-plain.svg" alt=""> CSS</li>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" alt="" /> React.js</li>
                </ul>
            </div>
        </div>
    </section>
</template>

<style scoped>
h2{
    margin-bottom: 3rem;
}

.project-group{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}
.project{
    width: 25vh;
    margin: 1rem 5rem;
    margin-bottom: 5rem;
    text-align: center;
    border-bottom: 4px solid #0F9410;
}

.main-img{
    width: 100%;
}

h3, p, li{
    color: #0F9410;
}
img{
    width: 10px;
    filter: grayscale(.4);
    transition: .2s;
}
img:hover{
    filter: grayscale(0);
}
ul{
    margin-top: .5rem;
}
</style>
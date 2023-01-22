<template>
    <section id="projects">
        <h2>Projects</h2>
        <div class="project-group">
            
            <div class="project">
                <a href="https://rafaelpolicher.github.io/Calculator/"><img class="main-img" src="../../public/img/dev.png" alt=""></a>
                <h3>Dev-Residencial</h3>
                <p>Ficticional project to marketing and land sales in a condominium</p>
                <ul>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-plain.svg" alt=""> HTML</li>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-plain.svg" alt=""> CSS</li>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-plain.svg" alt=""> JavaScript</li>
                </ul>
            </div>
            <div class="project">
                <a href="https://rafaelpolicher.github.io/dev-residencial/"><img class="main-img" src="../../public/img/calc.png" alt=""></a>
                <h3>Calc</h3>
                <p>An complete caulculator</p>
                <ul>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-plain.svg" alt=""> HTML</li>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-plain.svg" alt=""> CSS</li>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-plain.svg" alt=""> JavaScript</li>
                </ul>
            </div>
            <div class="project">
                <img class="main-img" src="../../public/img/soon.jpg" alt="">
                <h3>Soon</h3>
                <p>An React project</p>
                <ul>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-plain.svg" alt=""> HTML</li>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-plain.svg" alt=""> CSS</li>
                    <li><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-plain.svg" alt=""> React</li>
                </ul>
            </div>
        </div>
    </section>
</template>

<style scoped>
.project-group{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}
.project{
    width: 25vh;
    margin: 1rem 5rem;
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
}
</style>
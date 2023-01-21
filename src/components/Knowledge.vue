<template>
    <div id="knowledge">
        <h1>Knowledge</h1>
        <div class="knowledge-img">
            <div class="knowledge-group">
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-plain.svg" />
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-plain.svg" />
                <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-plain.svg" />
            </div>
          <div class="knowledge-group">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuejs/vuejs-original.svg" />
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" />
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-plain.svg" />
        </div>

        </div>
    </div>
</template>
<style scoped>
    #knowledge{
        height: 80vh;
        border-bottom: 1px solid green;
    }
    h1{
    color:#6C0094;
    margin-left: 2rem;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    font-size: 3rem;    
    display: flex;
    justify-content: center;
    margin-top: 5rem;
}

.knowledge-group{    
    display: flex;
    justify-content: center;
    margin: 5rem;
    color: white;
}

img{
    width: 25vh;
    margin: 0 5rem;
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
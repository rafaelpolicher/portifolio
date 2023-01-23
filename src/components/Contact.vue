<template>
    <section id="contact">
        <div >
            <p>Developed by Rafael Policher</p>
        </div>
        <div >
            <p><img src="../../public/img/linkedin.png" alt=""> <a href="https://www.linkedin.com/in/rafael-policher-36651724a" target="_blank">Rafael Policher</a></p>
            <p><img src="../../public/img/gmail.png" alt=""> Rafaelpolicher@gmail.com</p>
        </div>
    </section>
</template>

<style scoped>
#contact{
    height: 150px;
}
section{
    display: flex;
    justify-content: space-around;
}
div{
    margin-top: 2rem;
}
a{
    color: darkgray;
    transition: .2s;
    border-bottom: 1px solid transparent;
}
a:hover{
    border-bottom: 1px solid #0F9410;
}
p{
    color: darkgray;
    margin: 1rem 0 1rem 0;
    text-align: center;
}
img{
    width: 15px;
}
</style>
<template>
    <nav class="nav-menu">
        <i class="fas fa-bars" @click="showMenu()"></i>
        
        <div class="nav-content" :class="this.showMobileMenu ? 'open-menu' : 'closed-menu'">
            <ul class="nav-content">
                <li><a href="#home">Home
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                </a></li>
                <li><a href="#about">About
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                </a></li>
                <li><a href="#knowledge">Knowledge
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span></a></li>
                <li><a href="#projects">Projects
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                </a></li>
                <li><a href="#contact">Contact
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                </a></li>
            </ul>
        </div>
    </nav>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.nav-menu{
    background: black;
    height: 15vh;
    overflow: hidden;
    position: fixed; 
    top: 0; 
    width: 100%;
    z-index: 100;

}
.nav-content{
    display: flex;
    justify-content: flex-end;
    height: 100%;
    align-items: center;
}
li{
    margin: .5rem;
    margin-top: .5rem;
}
a{
    color: #6C0094;
    border: 1px solid transparent;
    border-bottom: 1px solid #0F9410;
    padding: .5rem;
    transition: .7s;
    position: relative;
    text-transform: uppercase;
    letter-spacing: .5rem;
}
/*a:hover{
    color:#220794;
    border: 1px solid #0F9410;
    border-radius: 5px;
}*/

a span{
    position: absolute;
    display: block;
    background: #0F9410;
}

a span:nth-child(1){
    left: 0;
    top: 0;
    width: 50.5%;
    height: 1px;
    transform: scaleX(0);
    transform-origin: left;
    transition: transform .1s;
    transition-delay: .1s;
}
a:hover span:nth-child(1){
  transform: scaleX(1);
  transform-origin: left;
}

a span:nth-child(2){
    right: 0;
    top: 0;
    width: 50.5%;
    height: 1px;
    transform: scaleX(0);
    transform-origin: right;
    transition: transform .1s;
    transition-delay: .1s;
}
a:hover span:nth-child(2){
  transform: scaleX(1);
  transform-origin: right;
}

a span:nth-child(3){
    right: 0;
    top: 0;
    width: 1px;
    height: 100%;
    transform: scaleY(0);
    transform-origin: bottom;
    transition: transform .1s;
}
a:hover span:nth-child(3){
  transform: scaleX(1);
  transform-origin: bottom;
}

a span:nth-child(4){
    left: 0;
    top: 0;
    width: 1px;
    height: 100%;
    transform: scaleY(0);
    transform-origin: bottom;
    transition: transform .1s;
}
a:hover span:nth-child(4){
  transform: scaleX(1);
  transform-origin: bottom;
}
.label-menu, .checkbox{
    display: none;
}

@media screen and (max-width: 830px) {
    .nav-menu {
padding-top: 10px;
position: absolute;
width: 100%;
}
.open-menu {
opacity: 1;
height: 150px;
}
.closed-menu {
opacity: 0;
height: 0;
padding: 0;
}
.nav-content {
flex-direction: column;
z-index: 100;
position: relative;
transition: all 0.2s ease-out;
}
.nav-items {
flex-direction: column;
}
i {
display: block;
text-align: right;
padding: 0 10px 10px 0;
}

}
</style>
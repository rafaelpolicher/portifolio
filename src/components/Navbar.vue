<template>
    <nav>
        <ul>
            <li><a href="#about">About
                <span></span>
                <span></span>
                <span></span>
                <span></span>
            </a></li>
            <li><a href="#knowledge">Knowledge                         <span></span>
                <span></span>
                <span></span>
                <span></span></a></li>
            <li><a href="#">Projects
                <span></span>
                <span></span>
                <span></span>
                <span></span>
            </a></li>
            <li><a href="#">Contact
                <span></span>
                <span></span>
                <span></span>
                <span></span>
            </a></li>
        </ul>
    </nav>
</template>

<script>
export default {
    
}
</script>

<style >
nav{
    background: black;
    height: 20vh;
    border-bottom: 1px solid grey;
}
ul{
    display: flex;
    justify-content: flex-end;
    height: 100%;
    align-items: center;
}
li{
    margin: .5rem;
}
a{
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    color: #6C0094;
    border: 1px solid transparent;
    border-bottom: 1px solid #0F9410;
    padding: .5rem;
    transition: .7s;
    position: relative;
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
</style>
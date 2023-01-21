<template>
    <nav>
        <ul>
            <li><a href="#about">About</a></li>
            <li><a href="#knowledge">Knowledge</a></li>
            <li><a href="#">Projects</a></li>
            <li><a href="#">Contact</a></li>
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
    border: 1px solid black;
    border-bottom: 1px solid #0F9410;
    padding: .5rem;
    transition: .7s;
    
}
a:hover{
    color:#220794;
    border: 1px solid green;
    border-radius: 5px;
}
</style>
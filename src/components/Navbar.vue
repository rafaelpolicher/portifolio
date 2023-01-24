<!----><template>
    <nav class="nav-menu"> 
        <button class="button-mobile" @click="showMenu()">Menu</button>
            <div class="nav-content">
                <ul class="nav-items" :class="this.showMobileMenu ? 'open-menu' : 'closed-menu'">
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
        data() {
            return {
                showMobileMenu: false,
                };
        },
        methods: {
            showMenu() {
                this.showMobileMenu = !this.showMobileMenu;
            },
        },
    };
</script>

<style scoped>
button{
    background: white;
}
.nav-menu{
    background: black;
    position: fixed; 
    width: 100%;
    z-index: 1;
}
.nav-items{
    display: flex;
    justify-content: flex-end;
    align-items: center;
    height: 15vh;
}
li{
    margin: .5rem;
    margin-top: 1rem;
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
.button-mobile{
    width: 50px;
    height: 50px;
    background: white;
    border-radius: 50%;
    display: none;
    cursor: pointer;
}


@media screen and (max-width: 830px) {
    .button-mobile{
    display: block;
}

.nav-content{
    justify-content: center;
    }
    li{
        margin: 1rem;
    }
    a , li{
        background: transparent;
    }

    .open-menu{
        opacity: 1;
        flex-direction: column;
        justify-content: center;
        height: 300px;
        background-image: linear-gradient(to bottom, black, #141414);
    }

    .closed-menu{
        opacity: 0;
        display: none;
        height: 0px;
        width: 0;
    }

}
</style>
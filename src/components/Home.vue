<template>
    <main id="home">
      <div class="img-mobile" v-motion-slide-visible-right>
            <img src="../../public/img/photo.jpg" alt="">
        </div>
        <div class="title" v-motion-fade>
            <h1>Hi, I am Rafael Policher</h1>
            <h1 class="writer">
                <span class="typed-text">{{ typeValue }}</span>
                <span class="blinking-cursor">|</span>
                <span class="cursor" :class="{ typing: typeStatus }">&nbsp;</span>
            </h1>
            <div class="social">
                <ul>
                    <li><a href="https://www.linkedin.com/in/rafael-policher-36651724a" target="_blank">Linkedin</a></li>
                    <li><a href="https://github.com/rafaelpolicher" target="_blank">GitHub</a></li>
                </ul>
            </div>
        </div>
        <div class="img" v-motion-slide-visible-right>
            <img src="../../public/img/photo.jpg" alt="">
        </div>
        
    </main>
</template>

<script>
export default {
    data: () => {
    return {
      typeValue: "",
      typeStatus: false,
      displayTextArray: ["Front-End Developer", "Web Developer"],
      typingSpeed: 100,
      erasingSpeed: 100,
      newTextDelay: 2000,
      displayTextArrayIndex: 0,
      charIndex: 0,
    }
  },
  methods: {
    typeText() {
      if (this.charIndex < this.displayTextArray[this.displayTextArrayIndex].length) {
        if (!this.typeStatus) this.typeStatus = true;
        this.typeValue += this.displayTextArray[this.displayTextArrayIndex].charAt(
          this.charIndex
        );
        this.charIndex += 1;
        setTimeout(this.typeText, this.typingSpeed);
      } else {
        this.typeStatus = false;
        setTimeout(this.eraseText, this.newTextDelay);
      }
    },
    eraseText() {
      if (this.charIndex > 0) {
        if (!this.typeStatus) this.typeStatus = true;
        this.typeValue = this.displayTextArray[this.displayTextArrayIndex].substring(
          0,
          this.charIndex - 1
        );
        this.charIndex -= 1;
        setTimeout(this.eraseText, this.erasingSpeed);
      } else {
        this.typeStatus = false;
        this.displayTextArrayIndex += 1;
        if (this.displayTextArrayIndex >= this.displayTextArray.length)
          this.displayTextArrayIndex = 0;
        setTimeout(this.typeText, this.typingSpeed + 1000);
      }
    },
  },
  created() {
   setTimeout(this.typeText, this.newTextDelay + 200);
},
}
</script>

<style scoped>
main{
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 80vh;
    border-bottom: 1px solid #0F9410;
}
h1, .writer{
    color:#6C0094;
    margin-left: 2rem;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    font-size: 3rem;
}
/*.writer::after{
    content: "|";
    margin-left: 5px;
    opacity: 1;
    color: grey;
    background-color: grey;
    animation: blink 1s infinite
}*/
.blinking-cursor{
    color: gray;
    animation: blink 1s infinite
}


@keyframes blink{
    0%{
        opacity: 1;
    }
    100%{
        opacity: 0;
    }
}

ul{
    display: flex;
    height: 100%;
    margin-top: 1rem;
    margin-left: 4rem;
}
li{
    margin: .5rem;
}
a{
  border: 1px solid #0F9410;
  color: #6C0094;
    border-radius: 10px;
    padding: .5rem 3rem;
    text-transform: uppercase;
    transition: .3s;
    letter-spacing: .3rem;
}
a:hover{
    background: #6C0094;
    color: black;
}
img{
    height: 15rem;
    border-radius: 50%;
    margin-right: 5rem;
}
.img-mobile{
  display: none;
}
@media screen and (max-width: 830px) {
#home{
  display: block;

}
  .img{
    display: none;
    }
  .img-mobile{
    display: block;
    text-align: center;
  }
  .img-mobile img{
    margin: 2rem;
    margin-top: 5rem;
  }

  h1, .writer{
    color:#6C0094;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    font-size: 2rem;
    text-align: center;
}
h1{
  margin-top: 2rem;
}

.writer{
  margin-bottom: 2rem;
}

.social{
  display: flex;
  justify-content: center;
}
a{
    color: #6C0094;
    padding: .7rem 1rem;
    text-transform: uppercase;
    transition: .3s;
    letter-spacing: .15rem;
}

}
</style>
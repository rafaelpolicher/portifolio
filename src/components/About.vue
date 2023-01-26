<template>
    <section id="about" v-motion-slide-visible-left>
        <h2>About</h2>
        <p>Passionate about technology and a beginner in web development.
 I had my first contact with development in a tech course in 2011. In 2016 I entry in Military Police, and now, after 7 years I'm changing careers.
Years of experience in a military environment brought several soft skills, such as interpersonal relationships, being a team player, communication, resilience, and the ability to work under pressure.
I'm self-taught in programming, studying through documentation and courses like <a href="../../public/certificate.pdf" download="../../public/certificate.pdf">Web Design for Everybody: Basics of Web Development & Coding at the University of Michigan ⇩.</a>
 As a beginner, I'm willing to learn other technologies and ready to take a step forward working in a team of developers.
</p>
    </section>
</template>

<style scoped>

a{
    text-decoration: underline;
    color: #785394;
}

p{
    margin: 4rem;
    margin-bottom: 7rem;
    color: #785394;
    text-align: center;
    font-size: 1.5rem;
}

@media screen and (max-width: 830px) {
    #about{
        margin: -2rem;
        margin-top: 10rem;
        border-top: 1px solid green;
    }
}
</style>
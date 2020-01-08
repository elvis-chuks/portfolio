<template>
    <div id="aboutme">
    <h1 heady>
        Hello! &#127757;,
    </h1>

    <div pagey>
        <p>My name is Elvis Chuks, I am a Software Engineer and i love making things that might possibly work using Python &#128013; / Golang &#128059;. I also play the guitar and piano in my leisures as i enjoy music a lot</p>
        <p>I've built products for companies and businesses around the globe ranging from basic websites to complex solutions and enterprise apps with focus on fast, elegant and accessible user experiences.</p>
        <p>Most recently, I was a Back end engineering contractor with PeaceMass Transit (one of Nigerias foremost public transportation company) building Elegant software applications to cater for their services.</p>
        <p>I'm now available for contracts and remote full-time roles. Want us to work together? You should <a class="contact-link" href="#"><u>contact me </u>&#128521;</a>.</p>
    </div>
    <!-- I've built products for companies and businesses around the globe ranging from basic websites to complex solutions and enterprise apps with focus on fast, elegant and accessible user experiences.

Most recently, I was a Senior front end engineering contractor with Pixel2HTML building JavaScript applications and interfaces for orgs and individuals.

Before then, I led the front end engineering team at Conectar LLC through building multiple React applications into a single powerful online learning platform. I deliver quality stuff contracting with these organizations internationally. I also created the Palenight theme for VS Code which has seen hundreds of thousands of downloads.

I'm now available for contracts and remote full-time roles. Want us to work together? You should -->
    </div>
</template>

<script>
export default {
    name: "ExperienceLeft"
}
</script>

<style scoped>

#aboutme{
    margin-top: 130px;
    margin-bottom: 150px;
}
@media (max-width: 576px) { 
    #aboutme{
        margin-bottom: 0px;
    }
}
[heady]{
    margin-top:30px;
    font-weight: bold;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;

}
[pagey]{
    margin-top:30px;
    font-size: 17px;
    font-weight: 500;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}

a{
    color: #330033;
    /* text-decoration:underline; */
}
a:hover{
    color:black;
}
</style>
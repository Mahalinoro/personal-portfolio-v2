<template>
  <section class="section designs">
    <div class="container pl-6 pr-6 pt-6">
      <div class="columns  mb-6">
          <div class="column m-right">
              <h1 class="title">Design</h1>
              <svg class="rect-pos" width="150" height="5" viewBox="0 0 150 5" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <rect width="150" height="5" fill="#E0115F"/>
              </svg>

              <p class="about-text mb-4">Some of the designs that I worked on. All of these have been designed using Figma.</p>
          </div>

          <div class="column">
            <div class="card">
              <div class="card-image">
                <figure class="image opac">
                  <img src="~/assets/universal.png" alt="Placeholder image">
                </figure>
              </div>
              <div class="card-content">
                <div class="content wi">
                  <p class="title is-6">My Universal Portfolio</p>
                  <a class="icopos">
                    <img src="~/assets/link10x.png">
                  </a>
                </div>
              </div>
            </div>
          </div>
      </div>

      <div class="columns is-multiline is-mobile">
      <div v-for="design of designs" class="column is-half">
        <div class="card">
            <div class="card-image">
              <figure class="image opac">
                <img v-bind:src="design.source" alt="Placeholder image">
              </figure>
            </div>
            <div class="card-content">
              <div class="content psm">
                <p class="title is-6">{{design.title}}</p>
                <a v-bind:href="design.demo" class="icosm">
                  <img src="~/assets/link10x.png">
                </a>
              </div>
            </div>
          </div>
      </div>
    </div>
     
    </div>
  </section>


</template>

<script>
export default {
  data() {
      return {
        designs: [
           {
             title: 'Miahy Mental Health Services',
             demo: 'https://www.figma.com/file/TKoMpKAiph5ImuwnrBs6bI/MIAHY?node-id=0%3A1',
             source: 'miahy.png'
           },
           {
             title: 'Otaku Zone',
             demo: 'https://www.figma.com/file/i4OUYerEHK6DvVSflLX3vk/OtakuZone-Design?node-id=0%3A1',
             source: 'otakuzone.png'
           },
           {
             title: "Neba's portfolio",
             demo: 'https://www.figma.com/file/2sqhhyGvh9rgKRw7Jne5Hu/Neba-s-portfolio?node-id=0%3A1',
             source: 'neba.png'
           },
           {
             title: 'Personal Portfolio V2',
             demo: 'https://www.figma.com/file/w5gDhRciZcLcjqcpXNAacw/Second-Portfolio?node-id=1%3A2',
             source: 'v2.png'
           },
        ]
      }
    },
}

</script>

<style lang='scss'>
 .designs{
        background: rgba(41, 41, 49, 0.86);
  }

  .opac{
    opacity: 0.6;
  }

  .icopos{
    position: relative;
    bottom: 35px;
    left: 430px;
  }

  .wi{
    height: 18px;
  }

  .icosm{
    position: relative;
    bottom: 35px;
    left: 430px;
  }

  .psm{
    height: 15px;
  }

  .card:hover{
    filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
  }

  .image:hover{
    opacity:1;
  }

@media only screen and (max-width: 600px) {

}
</style>

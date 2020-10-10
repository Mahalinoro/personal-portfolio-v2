<template>
  <section class="section main">
    <div class="container">
      <div class="columns">
        <div class="column">
          <div class="columns move-down">
            <div class="column is-one-quarter is-one-fifth-mobile down">
                <ul>
                  <li>
                    <a>
                    <figure class="image is-16x16 mb-5">
                      <img src="~/assets/linkedin.png">
                    </figure>
                    </a>
                  </li>
                  <li>
                   <a>
                   <figure class="image is-16x16 mb-5">
                      <img src="~/assets/github.png">
                    </figure>
                    </a>
                  </li>
                  <li>
                   <a>
                    <figure class="image is-16x16 mb-5">
                      <img src="~/assets/dribble.png">
                      </figure>
                    </a>
                  </li>
                  <li>
                   <a>
                    <figure class="image is-16x16 mb-5 img">
                      <img src="~/assets/twitter.png">
                      </figure>
                    </a>
                  </li>                
                </ul>
                <svg class="move-right" width="4" height="191" viewBox="0 0 4 191" fill="none" xmlns="http://www.w3.org/2000/svg">
                <rect width="4" height="191" fill="#E0115F"/>
                </svg>

            </div>

            <div class="column move-up">
                <img class="laptop" src="~/assets/laptop.png">
            </div>
            </div>
        </div>

        <div class="column mt-4">
          <p class="pinky mb-3">Hello, my name is:</p>
          <p class="large-text">Mahalinoro Razafimanjato<span> _</span></p>
          <p class="large-text-grey mb-5">A Tech Enthusiast<span> _</span></p>
          <p class="small-text mb-5">Currently, I am a third-year student in Computer Science at The African Leadership University. I am into Python Programming, Web Development, Data Science and UI Design. </p>
            <nuxt-link to="/contact" class="button bl">
                <span>Get in Touch</span>
            </nuxt-link>
        </div>
      </div>
    </div>
  </section>


</template>

<script>
export default {

}
</script>

<style lang='scss'>
  .main{
    background: linear-gradient(180deg, #292931 60.55%, rgba(41, 41, 49, 0.86) 93.62%);
    height: 550px;
  }

  .laptop{
    width:340px;
    height:auto;
  }

  .pinky{
    color:#E0115F;
    font-weight:normal;
    letter-spacing: 0.05em;
    font-size: small;
  }

  .large-text{
    font-weight: bold;
    color: #EAEAE9;
    font-size: 280%;
  }

  .large-text span{
    color:#E0115F;
    font-weight: 200;
  }


  .large-text-grey span{
    color:#E0115F;
    font-weight: 200;
  }

  .large-text-grey{
    font-weight: 600;
    color: rgba(234, 234, 233, 0.7);
    font-size: 240%;
  }

  .small-text{
    color: rgba(234, 234, 233, 0.7);
    font-weight: normal;
    width: 80%;
    font-size: normal;
  }

  .bl{
    background:#E0115F;
    color: #292931;
    font-weight: 500; 
  }

  .bl:hover{
    color: #292931;
  }

  .move-down{
      position:relative;
      top:90px
  }

  .move-right{
    position: relative;
    left:4px
  }

  .down{
    position:relative;
    top: 35px
  }

  @media only screen and (max-width: 600px) {
      .main{
        height: 750px;
      }
      .laptop{
        width:200px;
        height:auto;
      }

      .move-down{
        position: relative;
        top: -60px;
      }

      .resize{
        width: 50px;
        height: auto;
        margin: 0px;
      }

      .move-up{
        position: absolute;
        bottom: 50px;
        left: 70px;
      }

    .large-text{
      font-size: 150%;
    }

    .large-text-grey{
      font-size: 100%
    }

    .small-text{
      width: 80%;
      font-size: x-small;
    }

    .bl{
      width: 30%;
      height: auto;
      font-size: small;
    }

  }
</style>

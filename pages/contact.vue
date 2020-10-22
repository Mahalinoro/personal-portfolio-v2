<template>
  <section class="section contact">
    <div class="container">
    <div class="columns is-mobile">
      <div class="column is-half is-offset-one-quarter">
        <svg class="le" width="150" height="5" viewBox="0 0 150 5" fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect width="150" height="5" fill="#E0115F"/>
        </svg>
        <h1 class="title ce">Get in Touch</h1>
        <svg class="ri" width="150" height="5" viewBox="0 0 150 5" fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect width="150" height="5" fill="#E0115F"/>
        </svg>
        <p class="simple-text mb-6 ce">Feel free to contact me if you have any questions, comments or feedback. I am also looking for new opportunities to improve on my skills, 
        if you have any please don’t hesitate to reach out to me!</p>

        <form class="gform" name="contact" netlify-honeypot="bot-field" action="/thank-you" method="post" netlify>
        <input type="hidden" name="form-name" value="contact" />
        <p class="hidden">     
          <label>Don’t fill this out: <input name="bot-field"></label>   
        </p>
          <div class="field is-horizontal">
            <div class="field-body">
              <div class="field">
                <p class="control is-expanded">
                  <input class="input" name="Name" type="text" placeholder="Name*">
                </p>
              </div>
              <div class="field">
                <p class="control is-expanded">
                  <input class="input" name="Email" type="email" placeholder="Email*">

                </p>
              </div>
            </div>
          </div>

          <div class="field is-horizontal">
            <div class="field-body">
              <div class="field">
                <div class="control">
                  <input class="input" name="Subject" type="text" placeholder="Subject*">
                </div>
              </div>
            </div>
          </div>

          <div class="field is-horizontal">
            <div class="field-body">
              <div class="field">
                <div class="control">
                  <textarea class="textarea" name="Message" placeholder="Message*"></textarea>
                </div>
              </div>
            </div>
          </div>

          <div class="field is-horizontal mt-5">          
            <div class="field-body">
              <div class="field has-text-centered">
                <div class="control">
                  <button class="button">
                    Submit
                  </button>
                </div>
              </div>
            </div>
          </div>
        </form>
      </div>
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
  .contact{
       background: linear-gradient(180deg, #292931 60.55%, rgba(41, 41, 49, 0.86) 93.62%);
  }

  .ce{
    text-align:center !important;
  }

  .le{
    position:relative;
    top:30px;
    right: -20px;
  }

  .ri{
    position:relative;
    bottom: 53px;
    left: 400px;
  }

  .gform{
    margin:auto;
    width: 500px;
    height: auto;
  }

  .hidden {
  display: none;
}

.simple-text{
      color: rgba(234, 234, 233, 0.6);
    font-weight: normal;
    font-size: normal;
}


</style>

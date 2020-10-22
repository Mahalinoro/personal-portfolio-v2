<template>
    <div class="big">
        <div class="notification c">
            <p class="text">Thank you!</p>
            <p class="about-text mb-4">Will get back to you soon!</p>
            <nuxt-link to="/" class="button">
                Go Back to Home
            </nuxt-link>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang='scss'>
    .big{
        background: rgba(41, 41, 49, 0.86);
        height: 100vh;
    }

    .c{
        margin: auto;
        width: 30%;
        padding: 10px;
        top: 25%;
    }

    .text{
        color: #EAEAE9;
        font-weight: bold;
        font-size: 20px;
    }



  @media only screen and (max-width: 600px) {
      
  }
</style>

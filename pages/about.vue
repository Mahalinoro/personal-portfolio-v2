<template>
    <section class="section about">
        <div class="container pl-6 pr-6 pt-6">
            <div class="columns rez">
                <div class="column m-right">
                    <h1 class="title">About Me</h1>
                    <svg class="rect-pos" width="150" height="5" viewBox="0 0 150 5" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <rect width="150" height="5" fill="#E0115F"/>
                    </svg>

                    <p class="about-text mb-4">I am Mahaly, a tech enthusiast living in Madagascar the home of lemurs.</p>
                    <p class="about-text mb-4">I am a junior Computer Science student at <span>African Leadership University</span> based in Kigali, Rwanda. I enjoy designing (web pages, posters, social media posts, etc.). 
                    I have a passion for Python programming and I love sharing that with my local community through meetups.</p>
                    <p class="about-text mb-4">My goal is to create digital solutions to solve problems in my community as well as for the whole African continent.</p>
                    <p class="about-text pink mb-4">Tech Stacks:</p>

                    <div class="tile is-ancestor is-1">
                        <div class="tile is-parent pr-0">
                            <span class="button is-small">Python</span>
                        </div>
                        <div class="tile is-parent pr-0">
                            <span class="button is-small">Flask</span>
                        </div>
                        <div class="tile is-parent pr-0">
                           <span class="button is-small">HTML & CSS</span>
                        </div>

                    </div>

                    <div class="tile is-ancestor is-1">
                        <div class="tile is-parent pr-0">
                            <span class="button is-small">Ruby</span>
                        </div>
                        <div class="tile is-parent pr-0">
                            <span class="button is-small">Rails</span>
                        </div>
                        <div class="tile is-parent pr-0">
                            <span class="button is-small">PHP</span>
                        </div>

                    </div>
                </div>

                <div class="column h">
                    <img class="profile" src="~/assets/profile.png">
                    <svg class="large-pos" width="320" height="339" viewBox="0 0 320 339" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <rect width="320" height="339" rx="10" fill="#E0115F" fill-opacity="0.9"/>
                    </svg>
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
    .about{
        background: linear-gradient(180deg, #292931 60.55%, rgba(41, 41, 49, 0.86) 93.62%);
    }

    .about-text{
        color: rgba(234, 234, 233, 0.6);
        font-weight: normal;
        font-size: normal;
        width: 80%;
    }

    .about-text span, .pink{
        color: #E0115F;
    }

    .profile{
        position: relative;
        top: 100px;
        left: 50px;
        z-index: 1;
    }

    .rect-pos{
        position: relative;
        bottom: 55px;
        left: 150px;
    }

    .large-pos{
        position: relative;
        bottom: 280px;
        left: 80px;
    }

    .m-right{
        position: relative;
        left: 50px;
    }

    .rez{
        height: 550px;
    }


    @media only screen and (max-width: 600px) {
        .about-text{
        font-size: small;
        width: 100%;
        }

        .profile{
            top: 100px;
            left: 20px;
        }

        .rect-pos{
            width: 50px;
        }

        .large-pos{
            left: 40px;
            bottom: 250px;
            width: 200px;
        }

        .m-right{
            left: 5px;
            bottom: 50px
        }

        .rez{
            height: 550px;
        }

        .profile{
            left: 5px;
            top: 5px;
        }

        .rez{
            height: 1050px;
        }

        .h{
            height: 360px;
        }

    }
</style>
<template>
  <section class="section projects">
    <div class="container pl-6 pr-6 pt-6">
      <div class="columns mb-6">
        <div class="column m-right">
          <div class="card wd">
            <div class="card-content">
              <div class="media">
                <div class="media-content h-r">
                    <p class="title is-5 sz">PyladiesTNR Event Management System</p>
                    <div class="posx">
                      <a href="https://github.com/Mahalinoro/pyladies-web-app" class="mr-5">
                        <img src="~/assets/github10x.png">
                      </a>
                      <a href="https://mrazafiman.herokuapp.com/index.php">
                        <img src="~/assets/link10x.png">
                      </a>
                    </div>
                </div>
              </div>

              <div class="content">
                <p class="projects-text">A web application to manage Pyladies Antananarivo members for event signup. 
               Members can sign up for an event, signup to become a member, read blogpost, and access his/her personal dashboard. 
               Admin can add blogpost, create new event and manage members.</p>
                <br>
                <div class="tile is-ancestor is-1">
                    <div class="tile is-parent pr-0">
                        <span class="is-small pinky">PHP</span>
                    </div>
                    <div class="tile is-parent pr-0">
                        <span class="is-small pinky">MySQL</span>
                    </div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <div class="column m-right">
          <div class="r">
            <h1 class="title">Projects</h1>
            <svg class="rect-pos right" width="150" height="5" viewBox="0 0 150 5" fill="none" xmlns="http://www.w3.org/2000/svg">
                <rect width="150" height="5" fill="#E0115F"/>
            </svg>

          </div>
          <p class="about-text mb-4 a-right">Some of the works that I have built ranging from personal 
          projects to school based projects developed in collaboration with some of my classmates.</p>
        </div>
      </div>


    <div class="columns is-multiline is-mobile">
      <div v-for="project of projects" class="column is-one-third">
        <div class="card">
            <div class="card-content">
              <div class="media">
                <div class="media-content h-m">
                    <p class="title is-6 sm">{{ project.title }}</p>
                    <div class="posm">
                      <a v-bind:href="project.github" class="mr-4">
                        <img src="~/assets/github10x.png">
                      </a>
                      <a v-bind:href="project.demo">
                        <img src="~/assets/link10x.png">
                      </a>
                    </div>
                </div>
              </div>

              <div class="content">
                <p class="projects-text-is-small hh">{{ project.description }}</p>
                <br>
                <div class="tile is-ancestor is-1">
                    <div  v-for="stack of project.tech" class="tile is-parent pr-0">
                        <span class="is-6 pinky">{{ stack }}</span>
                    </div>
                </div>
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
        projects: [
           {
             title: 'Anime Recommendation System',
             description: 'A console application to get anime/manga recommendation. Users can receive anime recommendation based on his/her preferences,  and get updates from the web (MyAnimeList.com) on airing animes.',
             github: 'https://github.com/Mahalinoro/anime-recommendation-sytem',
             demo: 'https://github.com/Mahalinoro/anime-recommendation-sytem',
             tech: ['Python', 'bs4']
           },
           {
             title: 'Movie ChatBot',
             description: 'An online chatbot that provides Movie the user information about a specific movie that has been requested. Using the IMDB API and DialogFlow to configurate small talk and intents.',
             github: 'https://github.com/Mahalinoro/movie-bot',
             demo: 'https://movie-bot-mrazaf.herokuapp.com/',
             tech: ['Python', 'Flask', 'DialogFlow']
           },
           {
             title: 'My Universal Portfolio',
             description: 'My first portfolio website that I designed using Ruby on Rails, HTML and simple CSS. It improved my design skill and helped me discover how to use Particles.js. It’s called “Universal” because the theme is based on stars and universe.',
             github: 'https://github.com/Mahalinoro/my-universal-portfolio',
             demo: 'https://mahalinoro-r.herokuapp.com/',
             tech: ['HTML/CSS', 'Ruby/Rails']
           },
           {
             title: 'Hacktoberfest x PyladiesTNR',
             description: 'A simple project that lets first-timers in the community to contribute to Open Source. To contribute, participant should add their name, fun facts and social media links in the data dictionary. Then a card will be dispayed showing the information they inserted.',
             github: 'https://github.com/PyladiesTNR/Hackotberfest-PyladiesTNR-2020',
             demo: 'https://pyladiestnr-hacktober.herokuapp.com/',
             tech: ['Python', 'Flask']
           },
           {
             title: 'Personal Portfolio V2',
             description: 'A second version of my personal portfolio. The intent of this simple project is to apply learnings and try out Vue.js/Nuxt.js and Bulma as the CSS Framework.',
             github: '#',
             demo: '#',
             tech: ['Vue.js', 'Nuxt.js', 'Bulma']
           },
            {
             title: 'Ticket & Food Ordering App',
             description: "This program we developed lets customers purchase movie ticket easy and fast. The customers can see all the avalaible movie screening at the cinema with the information, choose directly which one to watch and pay at the same time. It is not only about movie ticket, and they can buy foods and drinks.",
             github: '#',
             demo: '#',
             tech: ['Java']
           },
        ]
      }
    },
}
</script>

<style lang='scss'>
    .projects{
        background: rgba(41, 41, 49, 0.86);;
    }

    .a-right{
      text-align: right;
    }

    .r{
      position: relative;
      left: 110px;
    }

    .wd{
      width: 420px;
      height: auto;
    }

    .projects-text{
      font-weight: normal;
      font-size: normal;
      color: rgba(234, 234, 233, 0.6);
    }

    .projects-text-is-small{
      font-weight: normal;
      font-size: small;
      color: rgba(234, 234, 233, 0.6);
    }

    .sz{
      width: 200px;
    }

    .sm{
      width: 150px;
    }

    .posx{
      position: absolute;
      bottom: 295px;
      left: 300px;
    }

    .posm{
      position: absolute;
      bottom: 265px;
      left: 230px;
    }

  .h-r{
    height: 50px;
  }

  .h-m{
    height: 50px;
  }

  .hh{
    height:130px;
  }
  
@media only screen and (max-width: 600px) {

}
 
</style>

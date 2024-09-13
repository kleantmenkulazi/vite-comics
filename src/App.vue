<script>

export default {

  data() {
    return {
      message: 'Hello world',

      links:[
        {
          text : 'CHARACTERS',
          url : "href='#'",
          active: false, 
        },
        {
          text : 'COMICS',
          url : "href='#'",
          active: true,
        },
        {
          text : 'MOVIES',
          url : "href='#'",
          active: false,
        },
        {
          text : 'TV',
          url : "href='#'",
          active: false,
        },
        {
          text : 'GAMES',
          url : "href='#'",
          active: false,
        },
        {
          text : 'COLLECTIBLES',
          url : "href='#'",
          active: false,
        },
        {
          text : 'CHARACTERS',
          url : "href='#'",
          active: false,
        },
        {
          text : 'VIDEOS',
          url : "href='#'",
          active: false,
        },
        {
          text : 'FANS',
          url : "href='#'",
          active: false,
        },
        {
          text : 'NEWS',
          url : "href='#'",
          active: false,
        },
        {
          text : 'SHOP',
          url : "href='#'",
          active: false,
        }
      ]
    }
  },

  methods:{

  },
}

</script>

<template>

  <header>
    <!-- sezione nera -->
    <div class="black-section"></div>

    <div class="container flex">
      <!-- logo -->
      <img class="logo" src=" " alt="DC">

      <div class="col-60">
        <ul>
          <li v-for="(link, index) in links">
            <a :href="link.url"> {{ link.text }} </a>  
          </li>
        </ul>
      </div>

    </div>

  </header>

  <main>

    <div class="container">

      <!-- content -->
      <section>

      </section>

      <!-- prodotti -->
      <section>
        
      </section>

    </div>

  </main>

  <footer>

    <div class="container">

      <!-- footer top -->
      <section>

      </section>

      <!-- footer bottom -->
      <section>
        
      </section>

    </div>

    <!-- sezione nera -->
    <div class="black-section"></div>

  </footer>

</template>

<style scoped>

/* general */
.flex{
  display: flex;
  justify-content: space-between;
  align-items: center;
}

img{
  max-width: 100%;
}

/* header */

.col-60{
  width: 60%;
}

.logo{
  width: 60px;
}

.black-section{
height: 50px;
width: 100%;
background-color: #0E0E0E;
}

.active{
  color: #0082F9;
}

ul{
  padding: 0;

  list-style: none;

  display: flex;
  justify-content: center;
  align-items: center;
}

li a{
  font-family: "Roboto Condensed";
  font-weight: bold;
  font-size: 0.9rem;
  text-decoration: none;
  color: black;
  display: inline-block;
  padding: 10px;
}

a{
  margin-top: 30px;
  margin-bottom: 30px;
}

a .active{
border-bottom: 2px solid #0082F9;
}


</style>

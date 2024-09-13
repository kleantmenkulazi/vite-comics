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

<!-- content -->
<section class="bg-black">

  <div class="container">

    <section class="content flex">
        <div>
            --&gt Content goes here &lt--
        </div>
    </section>
    
  </div>

</section>

<!-- prodotti -->
<section class="bg-blue">

  <div class="content">
      <section>
        hello
      </section>
  </div>

</section>

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

.bg-blue{
  background-color: #0082F9;
}

.bg-black{
  background-color: #0E0E0E;
}

/* header */

.logo{
  width: 60px;
}

.black-section{
height: 50px;
width: 100%;
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

  color: rgb(67, 67, 67);

  display: inline-block;

  padding: 10px;
  padding-bottom: 30px;
  margin-top: 30px;
}

.active{
  color: #0082F9;
  border-bottom: 4px solid #0082F9;
}

/* content */

.content{
  font-family: "Roboto Condensed";
  font-size: 1.2rem;

  color: white;

  height: 100px;
}


</style>

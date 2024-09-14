<script>

export default {

  data() {
    return {
      links:[
        {
          text : 'CHARACTERS',
          url : '#',
          active: false, 
        },
        {
          text : 'COMICS',
          url : '#',
          active: true,
        },
        {
          text : 'MOVIES',
          url : '#',
          active: false,
        },
        {
          text : 'TV',
          url : '#',
          active: false,
        },
        {
          text : 'GAMES',
          url : '#',
          active: false,
        },
        {
          text : 'COLLECTIBLES',
          url : '#',
          active: false,
        },
        {
          text : 'CHARACTERS',
          url : '#',
          active: false,
        },
        {
          text : 'VIDEOS',
          url : '#',
          active: false,
        },
        {
          text : 'FANS',
          url : '#',
          active: false,
        },
        {
          text : 'NEWS',
          url : '#',
          active: false,
        },
        {
          text : 'SHOP',
          url : '#',
          active: false,
        }
      ],
      products:[
        {
          text : 'DIGITAL COMICS',
          url : '#',
          image: '/public/img/buy-comics-digital-comics.png',
        },
        {
          text : 'DC MERCHANDISE',
          url : '#',
          image: '/public/img/buy-comics-merchandise.png',
        },
        {
          text : 'SUBSCRIPTION',
          url : '#',
          image: '/public/img/buy-comics-subscriptions.png',
        },
        {
          text : 'COMIC SHOP LOCATOR',
          url : '#',
          image: '/public/img/buy-comics-shop-locator.png',
        },
        {
          text : 'DC POWER VISA',
          url : '#',
          image: '/public/img/buy-dc-power-visa.svg',
        },
      ]
    }
  },

  methods:{

  },
}

</script>

<template>

  <header>

    <div class="myContainer">

      <div class="d-flex justify-content-between align-items-center">

            <!-- logo -->
            <img class="logo" src="/img/dc-logo.png" alt="DC">

            <!-- lista link -->
            <div>
                <ul>
                  <li v-for="(link, index) in links" :key="index">
                    <a :href="link.url" :class="link.active ? 'active' : '' " class="header-link"> {{ link.text }}</a>  
                  </li>
                </ul>
            </div>
            
      </div>

    </div>

  </header>

  <main>

    <!-- content -->
    <section class="bg-black">

      <div class="myContainer">

        <section class="content">

        </section>
        
      </div>

    </section>

    <!-- prodotti -->
    <section class="bg-blue">

      <div class="myContainer">

            <ul class="mb-0 py-4">
              <li v-for="(product, index) in products" :key="index">

                <a :href="product.url" class="d-flex align-items-center">

                  <img class="product-img m-2" :src="product.image" :alt="product.text">
                  <span class="text-white product-text">
                    {{product.text}}
                  </span>

                </a>

              </li>
            </ul>

      </div>

    </section>

  </main>

  <footer>

      <!-- footer top -->
      <section class="footer-top">

        <div class="myContainer d-flex justify-content-between align-items-center pt-4">

          <!-- links -->
          <div class="d-flex">
              <!-- DC COMICS & SHOP -->
              <section class="me-4">
                  
                  <div>
                        <p class="list-title mb-2">DC COMICS</p>

                        <ul>
                          <li>
                            <a href=""> Characters</a>
                          </li>
                          <li>
                            <a href=""> Comics</a>
                          </li>
                          <li>
                            <a href=""> Movies</a>
                          </li>
                          <li>
                            <a href=""> TV</a>
                          </li>
                          <li>
                            <a href=""> Games</a>
                          </li>
                          <li>
                            <a href=""> Videos</a>
                          </li>
                          <li>
                            <a href=""> News</a>
                          </li>
                        </ul>
                  </div>
    
                  <div>
                        <p class="list-title mb-2">SHOP</p>
                        <ul>
                          <li>
                            <a href=""> Shop DC</a>
                          </li>
                          <li>
                            <a href=""> Shop DC Collectibles</a>
                          </li>
                        </ul>
                  </div>

              </section>

              <!-- DC -->
              <section class="me-4">
                  
                  <div>
                        <p class="list-title mb-2">DC</p>

                        <ul>
                          <li>
                            <a href=""> Term of Use</a>
                          </li>
                          <li>
                            <a href=""> Privacy Policy</a>
                          </li>
                          <li>
                            <a href=""> Ad choices</a>
                          </li>
                          <li>
                            <a href=""> Advertising</a>
                          </li>
                          <li>
                            <a href=""> Jobs</a>
                          </li>
                          <li>
                            <a href=""> Subscriptions</a>
                          </li>
                          <li>
                            <a href=""> Talent Workshops</a>
                          </li>
                          <li>
                            <a href=""> CPSC Certificates</a>
                          </li>
                          <li>
                            <a href=""> Ratings</a>
                          </li>
                          <li>
                            <a href=""> Shop Help</a>
                          </li>
                          <li>
                            <a href=""> Contact Us</a>
                          </li>
                        </ul>
                  </div>

              </section>

              <!-- SITES -->
              <section>
                  
                  <div>
                        <p class="list-title mb-2">SITES</p>

                        <ul>
                          <li>
                            <a href=""> DC</a>
                          </li>
                          <li>
                            <a href=""> MAD Magazine</a>
                          </li>
                          <li>
                            <a href=""> DC Kids</a>
                          </li>
                          <li>
                            <a href=""> DC Universe</a>
                          </li>
                          <li>
                            <a href=""> DC Power Visa</a>
                          </li>
                        </ul>
                  </div>

              </section>
          </div>
 
          <!-- immagine sfondo -->
          <img class="dc-sfondo" src="/public/img/dc-logo-bg.png" alt="DC">
          
        </div>

      </section>

      <!-- footer bottom -->
      <section class="footer-bottom">

        <div class="myContainer d-flex justify-content-between align-items-center">
          <button class="sign-up-button">
            SIGN-UP NOW!
          </button>

          <div class="d-flex align-items-center">

              <div class="text-primary fw-bold me-3">
              FOLLOW US
              </div>

              <img class="me-3" src="/public/img/footer-facebook.png" alt="facebook">
              <img class="me-3" src="/public/img/footer-twitter.png" alt="facebook">
              <img class="me-3" src="/public/img/footer-youtube.png" alt="facebook">
              <img class="me-3" src="/public/img/footer-pinterest.png" alt="facebook">
              <img src="/public/img/footer-periscope.png" alt="facebook">

          </div>
        </div>
        
      </section>

  </footer>

</template>

<style scoped>

/* general */

.bg-blue{
  background-color: #0082F9;
}

a{
  text-decoration: none;
  padding: 10px;
}

/* header */

.logo{
  width: 60px;
  padding: 20px 0;
}

ul{
  padding: 0;

  list-style: none;

  display: flex;
  justify-content: center;
  align-items: center;
}

li .header-link{
  font-family: "Roboto Condensed";
  font-weight: bold;
  font-size: 0.9rem;
  color: rgb(67, 67, 67);
  padding-bottom: 45px;
  transition: color 0.3s ease-in-out
}

.header-link.active,
.header-link:hover{
  color: #0082F9;
  border-bottom: 4px solid #0082F9;
}

/* content */

.content{
  height: 100px;
}

/* prodotti */

.product-text{
  font-size: 0.8rem;
}

.product-img{
  height: 35px;
}

/* footer */

.footer-top{
  background-image: url('/public/img/footer-bg.jpg');
  overflow: hidden;
  position: relative;
}

.dc-sfondo{
  width: 480px;
  position: absolute;
  right: 15%
}

.list-title{
  color: white;
  font-family: "Roboto Condensed";
  font-weight: bold;
}

.footer-top ul{
  display: inline-block;
}

.footer-top li a{
  padding: 0;
  font-size: 0.7rem;
  color: grey;
}

/* footer bottom */

.footer-bottom{
  background-color: #303030;
  padding: 20px 0;
}

.sign-up-button{
  background-color:#303030;
  color: white;
  border: 1px solid #0082F9;
  padding: 10px 15px;
}

.sign-up-button:hover{
  background-color:#0082F9;
}

.footer-bottom img{
width: 25px;  
}

</style>

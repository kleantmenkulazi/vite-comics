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
        image: '/img/buy-comics-digital-comics.png',
      },
      {
        text : 'DC MERCHANDISE',
        url : '#',
        image: '/img/buy-comics-merchandise.png',
      },
      {
        text : 'SUBSCRIPTION',
        url : '#',
        image: '/img/buy-comics-subscriptions.png',
      },
      {
        text : 'COMIC SHOP LOCATOR',
        url : '#',
        image: '/img/buy-comics-shop-locator.png',
      },
      {
        text : 'DC POWER VISA',
        url : '#',
        image: '/img/buy-dc-power-visa.svg',
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
          <img class="logo" src="/vue-dc-comics-1/img/dc-logo.png" alt="DC">

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

  <!-- jumbo + fumetti -->
  <section class="bg-black">

    <!-- jumbo + bottone -->
    <div class="jumbo"> </div>

    <div class="myContainer product-container pt-5 pb-4 text-center">

        <div class="section-label py-2 px-3 fw-bold fs-4">
            CURRENT SERIES
        </div>

        <div class="row">

          <div class="col-2 mb-5 text-start">

            <!-- immagine -->
            <div class="img-container mb-3">

            </div>
            <!-- titolo -->
            <div class="text-white card-title">
                ACTION COMICS
            </div>

          </div>

        </div>

        <div>
          <button class="load-more-button py-2 px-5 fw-bold">
            LOAD MORE
          </button>
        </div>

    </div>

  </section>

  <!-- striscia blu prodotti -->
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
        <img class="dc-sfondo" src="/img/dc-logo-bg.png" alt="DC">
        
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

            <img class="me-3" src="/img/footer-facebook.png" alt="facebook">
            <img class="me-3" src="/img/footer-twitter.png" alt="facebook">
            <img class="me-3" src="/img/footer-youtube.png" alt="facebook">
            <img class="me-3" src="/img/footer-pinterest.png" alt="facebook">
            <img src="/img/footer-periscope.png" alt="facebook">

        </div>
      </div>
      
    </section>

</footer>

</template>

<style lang="scss" scoped>

  // general
  .bg-blue{
  background-color: #0082F9;
  }

  a{
  text-decoration: none;
  padding: 10px;
  }

  ul{
  padding: 0;

  list-style: none;

  display: flex;
  justify-content: center;
  align-items: center;
  }

  // header 
  header{
    .logo{
      width: 60px;
      padding: 20px 0;
    };

    li .header-link{
      font-family: "Roboto Condensed";
      font-weight: bold;
      font-size: 0.9rem;
      color: rgb(67, 67, 67);
      padding-bottom: 45px;
      transition: color 0.3s ease-in-out;

        &.active,
        &:hover{
          color: #0082F9;
          border-bottom: 4px solid #0082F9;
        };

    };
  };

  // main
  main{

    /* prodotti */
    .jumbo{
      height: 300px;
      background-image: url('/img/jumbotron.jpg');
      background-repeat: no-repeat;
      background-position: top;
      background-size:cover;
    };
    .product-container{
      position: relative;

          .section-label{
          font-family: "Roboto Condensed";
          color: white;
          background-color: #0082F9;
          position: absolute;
          left: 0;
          top: -25px;
          };

          .img-container{
          width: 150px;
          height: 150px;
          background-color: white;
          };

          .card-title{
          font-size: 0.8rem;
          };

          .load-more-button{
          color: white;
          background-color: #0082F9;
          font-family: "Roboto Condensed";
          border: none;

              &:hover{
              color: #0082F9;
              background-color: white;
              };
          };
    };

    /* fascia blu */
    .product-text{
      font-size: 0.8rem;
    };
    .product-img{
      height: 35px;
    };
  };

  // footer
  footer{

    // general
    & ul{
      display: inline-block;

      & li a{
      padding: 0;
      font-size: 0.7rem;
      color: grey;
      };
    };

    // footer top
    .footer-top{
      background-image: url('/img/footer-bg.jpg');
      overflow: hidden;
      position: relative;
    
        .dc-sfondo{
        width: 480px;
        position: absolute;
        right: 15%
        };

        .list-title{
        color: white;
        font-family: "Roboto Condensed";
        font-weight: bold;
        };

    };

    // footer bottom
    .footer-bottom{
      background-color: #303030;
      padding: 20px 0;

      .sign-up-button{
        background-color:#303030;
        color: white;
        border: 1px solid #0082F9;
        padding: 10px 15px;

        &:hover{
          background-color:#0082F9;
        };
      };

      & img{
        width: 25px;  
      };

    };

  };

</style>
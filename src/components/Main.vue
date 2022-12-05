<script>

export default{
    data() {
      return {
      listaFumetti: [
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
    "price": "$19.99",
    "series": "Action Comics",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
    "price": "$3.99",
    "series": "American Vampire 1976",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
    "price": "$16.99",
    "series": "Aquaman",
    "type": "graphic novel"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
    "price": "$2.99",
    "series": "Batgirl",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$3.99",
    "series": "Batman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$2.99",
    "series": "Batman Beyond",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
    "price": "$3.99",
    "series": "Batman/Superman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
    "price": "$4.99",
    "series": "Batman/Superman Annual",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
    "price": "$5.99",
    "series": "Batman: The Joker War Zone",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
    "price": "$6.99",
    "series": "Batman: Three Jokers",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
    "price": "$4.99",
    "series": "Batman: White Knight Presents: Harley Quinn",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
    "price": "$16.99",
    "series": "Catwoman",
    "type": "graphic novel"
  }
    ],
      }
    }, methods: {
      script () {

      }
    },
}

</script>

<template>

    <section class="bg-fumetti">
        <img id="jumbo" src="../assets/img/jumbotron.jpg" alt="">
        <div class="container">
            <div class="avviso d-flex">
                <h3 class="m-0">CURRENT SERIES</h3>
            </div>
        </div>
        <div class="container">
            <div class="products-container">
                <div class="row row-cols-1 row-cols-md-6 g-4">
                    <div class="col" v-for="(fumetto, i) in listaFumetti" :key="i">
                        <div class="card-fumetti">
                            <img rel="stylesheet" :src="fumetto.thumb">
                            <div class="card-body">
                                <h5 class="card-title pt-4">{{fumetto.series}}</h5>
                                <p class="card-text">{{fumetto.type}}</p>
                                <span class="card-text">{{fumetto.price}}</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="d-flex py-5 justify-content-center">
            <div class="btn btn-primary px-5">Load More</div>
        </div>
    </section>
    
    <section>
        <div class="shop">
            <div class="card">
                <img class="immagini" src="../assets/img/buy-comics-digital-comics.png" alt="">
                <a href="#">DIGITAL COMICS</a>
            </div>

            <div class="card">
                <img class="immagini" src="../assets/img/buy-comics-merchandise.png" alt="">
                <a href="#">DC MERCHANDISE</a>
            </div>
            
            <div class="card">
                <img class="immagini" src="../assets/img/buy-comics-subscriptions.png" alt="">
                <a href="#">SUBSCRIPTION</a>
            </div>

            <div class="card">
                <img class="immagini" src="../assets/img/buy-comics-shop-locator.png" alt="">
                <a href="#">COMIC SHOP LOCATOR</a>
            </div>

            <div class="card">
                <img class="immagini" src="../assets/img/buy-dc-power-visa.svg" alt="">
                <a href="#">DC POWER VISA</a>
            </div>
        </div>      
    </section>

    <section id="img-sfondo-sezione">
        <div class="container">
            <div class="menu">
                
            </div>
            <div class="logo-bg">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </section>

    <section class="bg-footer">
        <div class="container">
            <div>
                <button type="button" id="sing-up" class="btn btn-outline-primary">SIGN-UP NOW!</button>
            </div>
            <div>
                <span><strong>FOLLOW US</strong></span>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use "../styles/general.scss" as * ;

#jumbo{
    height: 25rem;
    width: 100%;
}

#img-sfondo-sezione{
    background-image: url(../assets/img/footer-bg.jpg);
    height: 25rem;
    background-repeat: no-repeat;
    width: 100%;
    background-size: cover;
}
#sing-up{
    color: white;
}

.avviso{
    color: white;
    background-color: $Bg-main-secondo;
    position: relative;
    top: -20px;
    padding: 0 3rem;
}
.fumetti{
    padding: 3rem 0;
    background-color: $Bg-main-primo;
    color: $Bg-header;
}

.row{
    padding-top: 5rem;
}

.bg-fumetti{
    background-color: rgb(28, 28, 28);
}

.bg-footer{
    background-color: rgb(48, 48, 48);
    padding: 4rem;
    position: relative;
}
.shop{
    padding: 3rem;
    background-color: $Bg-main-secondo;
    color: $Bg-header;
    display: flex;
    justify-content: center;
}

.card{
    border: none;
    background-color: $Bg-main-secondo;
    display: block;
}
.card-fumetti{
    border: none;
    background-color: rgb(28, 28, 28);
    color: white;
    display: block;
}

.immagini{
    background-color: $Bg-main-secondo;
    width: 40px;
    object-fit: contain;
    height: 40px;
    margin-left: 3rem;
}

.container{
    display: flex;
    justify-content: space-between;
}

.logo-bg{
    position: relative;
    top: -55px;
}

a{
    text-decoration: none;
    color: white;
    padding-left: 1rem;
    padding-right: 1rem;
}

  
</style>

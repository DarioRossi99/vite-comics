<script>

export default{

};
</script>

<template>

    <section id="bg-sezione">
        <div class="container">
            <div class="fumetti">
                <h2>Content goes here</h2>
            </div>
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
                <a href="#">DIGITAL COMICS</a>
            </div>
            
            <div class="card">
                <img class="immagini" src="../assets/img/buy-comics-subscriptions.png" alt="">
                <a href="#">DIGITAL COMICS</a>
            </div>

            <div class="card">
                <img class="immagini" src="../assets/img/buy-comics-shop-locator.png" alt="">
                <a href="#">DIGITAL COMICS</a>
            </div>

            <div class="card">
                <img class="immagini" src="../assets/img/buy-dc-power-visa.svg" alt="">
                <a href="#">DIGITAL COMICS</a>
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
</template>

<style scoped lang="scss">
@use "../styles/general.scss" as * ;

#bg-sezione{
    background-color:$Bg-main-primo;
}

#img-sfondo-sezione{
    background-image: url(../assets/img/footer-bg.jpg);
    height: 30rem;
}
.fumetti{
    padding: 3rem 0;
    background-color: $Bg-main-primo;
    color: $Bg-header;
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

.immagini{
    background-color: $Bg-main-secondo;
    width: 40px;
    object-fit: cover;
    height: -webkit-fill-available;
}

.container{
    display: flex;
    justify-content: space-between;
}

.logo-bg{
    position: relative;
    top: -50px;
}

a{
    text-decoration: none;
    color: white;
    padding-left: 1rem;
    padding-right: 1rem;
}

  
</style>

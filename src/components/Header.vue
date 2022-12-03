<script>

export default{

};
</script>

<template>
  <section>

      <div class="container">
        <div>
          <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <div class="link">
          <ul>
            <a href="#">CHARACTERS</a>
            <a href="#">COMICS</a>
            <a href="#">MOVIES</a>
            <a href="#">TV</a>
            <a href="#">GAMES</a>
            <a href="#">COLLECTIBLES</a>
            <a href="#">VIDEOS</a>
            <a href="#">FANS</a>
            <a href="#">NEWS</a>
            <a href="#">SHOP</a>
          </ul>
        </div>
      </div>

  </section>
</template>

<style scoped lang="scss">
@use "../styles/general.scss" as * ;

  a{
    text-decoration: none;
    color: black;
  }
  .backGround{
    background-color: $Bg-header;
  }
  .container{
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem;
  }

  .link{
    width: 60%;
    display: flex;
    justify-content: space-between;
  }

  ul{
    display: contents;
  }
  .listaLink{
    display: flex;
    justify-content: space-between;
    width: 65%;
  }

</style>

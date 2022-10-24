<template>
  <div class="container">
    <div class="left_Side d-flex align-items-center">
      <p class="topic">Building things is our mission.</p>
    </div>
    <div class="right_Side ">
<!--      <div class="info_carousel">-->
<!--        <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">-->
<!--          <ol class="carousel-indicators">-->
<!--            <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>-->
<!--            <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>-->
<!--            <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>-->
<!--          </ol>-->
<!--          <div class="carousel-inner">-->
<!--            <div class="carousel-item active">-->
<!--                Title-->
<!--            </div>-->
<!--            <div class="carousel-item">-->
<!--                Title-->
<!--            </div>-->
<!--            <div class="carousel-item">-->
<!--                Title-->
<!--            </div>-->
<!--          </div>-->
<!--          <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">-->
<!--            <span class="carousel-control-prev-icon" aria-hidden="true"></span>-->
<!--            <span class="sr-only">Previous</span>-->
<!--          </a>-->
<!--          <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">-->
<!--            <span class="carousel-control-next-icon" aria-hidden="true"></span>-->
<!--            <span class="sr-only">Next</span>-->
<!--          </a>-->
<!--        </div>-->
<!--      </div>-->
    </div>
  </div>
</template>

<script>
export default {
  name: "MainPage"
}
</script>

<style scoped>
  .container{
    height: 646px;
    width: 1440px;
    display: flex;
    left: 0px;
    top: 80px;
    /*border:1px solid red;*/
  }
  .topic{
    font-style: normal;
    font-weight: 600;
    font-size: 72px;
    line-height: 84px;
    font-family: 'Work Sans';
    color: #292E3D;
  }
  .left_Side{
    width: 50%;
  }
  .right_Side{
    width: 50%;
    position: relative;
  }
  .info_carousel {
    position: absolute;
    width: 416px;
    height: 190px;
    left: 1024px;
    top: 456px;
    background-color: #3559C7;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 20px 10px 10px;
    gap: 20px;
  }
  .carousel_img{
    position: absolute;
    width: 416px;
    height: 190px;
    left: 1024px;
    top: 456px;
    background-color: #3559C7;
  }

  @media screen and (max-width: 480px ){
      .container{
        width: 100%;
        display: inline;
      }
      .left_Side{
        width: 100%;
        height: 50%;
        padding: 20px;
      }
      .right_Side{
        width: 100%;
        height: 50%;
      }
      .topic{
        font-size: 44px;
      }
  }

  @media screen and (max-width: 768px) {
    .container{
      width: 100%;
      display: inline;
    }
    .left_Side{
      width: 100%;
      height: 80%;
      padding: 20px;
    }
    .right_Side{
      width: 100%;
      height: 50%;
      display: none;
    }
    .topic{
      font-size: 46px;
    }
  }

  @media screen and (min-width: 992px){
    .container{
      width: 100%;
      display: flex;
    }
    .left_Side{
      width: 100%;
      padding: 20px;
    }
    .right_Side{
      width: 100%;
    }
    .topic{
      font-size: 56px;
    }
  }


</style>
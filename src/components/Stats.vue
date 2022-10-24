<template>
  <div class="container d-flex">
      <div class="left_side col-7">
        <div class="stats_section">
            <div class="stats">
              <div class="info_stats">
                <div class="icon_stats">
                  <img class="img" src="../assets/illus1.png" alt="">
                </div>
                <p class="count">123</p>
                <h5>Happy Clients</h5>
              </div>
              </div>
            <div class="stats2">
              <div class="info_stats">
                <div class="icon_stats">
                  <img class="img" src="../assets/illus2.png" alt="">
                </div>
                <p class="count">123</p>
                <h5>Projects Completed</h5>
              </div>
            </div>
        </div>
        <div class="stats_section">
            <div class="stats3">
              <div class="info_stats">
                <div class="icon_stats">
                  <img class="img" src="../assets/illus4.png" alt="">
                </div>
                <p class="count">123</p>
                <h5>Projects Completed</h5>
              </div>
            </div>
            <div class="stats4">
              <div class="info_stats">
                <div class="icon_stats">
                  <img class="img" src="../assets/illus3.png" alt="">
                </div>
                <p class="count">123</p>
                <h5>Years in Business</h5>
              </div>
            </div>
        </div>
      </div>
      <div class="right_side col-5">
          <div class="card_info">
            <div class="title">
              30 Years Experience
            </div>
            <div class="desc col-8">
              Our company has been the leading provided construction services to clients throughout the USA since 1988.
            </div>
            <div class="btn_info">
              Contact Us
            </div>
          </div>
     </div>
  </div>
</template>

<script>
export default {
  name: "Stats_"
}
</script>

<style scoped>
    .container{
      margin-top: 3vw;
      margin-bottom: 10vw;
      border:1px solid green;
      position: relative;
    }
    .left_side{
      width: 60%;
      position: relative;
      margin-top: 3vw;
      border: 1px solid red;
    }
    .right_side{
      width: 40%;
      border:1px solid black;
      margin-top: 3vw;
    }
    .title{
      font-family: 'Work Sans';
      font-style: normal;
      font-weight: 700;
      color: #2947A9;
      font-size: 60px;
      line-height: 70px;
    }
    .btn_info{
      width: 30%;
      color: #E0E3EB;
      font-weight: 600;
      border: none;
      padding: 2%;
      cursor: pointer;
      text-align: center;
      background-color: #3559C7;
    }
    .stats_section{
      display: flex;
    }
    .desc{
      margin-top: 2vw;
      margin-bottom: 2vw;
    }

    .stats{
      width: 361px;
      height: 125px;
      left: calc(50% - 361px/2 - 327.5px);
      box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
      border-radius: 5px;
      margin-top: 40px;
      background-color: #F6F8F7
    }
    .stats2{
      width: 279px;
      height: 125px;
      left: calc(50% - 361px/2 - 327.5px);
      box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
      border-radius: 5px;
      z-index: 999;
      position: absolute;
      margin-left: 500px;
      background-color: #F6F8F7;
    }
    .icon_stats{
      position: relative;
    }
    .img {
      left: 200px;
      top: -40px;
      position: absolute;
    }
    .stats .img {
      left: -50px;
      top: -60px;
    }

    .stats3 .img{
      top: 70px;
      left: 300px;
    }

    .stats3{
      width: 361px;
      height: 125px;
      left: calc(50% - 361px/2 - 327.5px);
      box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
      border-radius: 5px;
      margin-top: 50px;
      margin-left: 200px;
      z-index: 999;
      position: absolute;
      background-color: #F6F8F7;

    }
    .stats4{
      width: 301px;
      height: 125px;
      left: calc(50% - 361px/2 - 327.5px);
      box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
      border-radius: 5px;
      z-index: 99999;
      margin-top: 10px;
      margin-left: 480px;
      position: absolute;
      background-color: #F6F8F7;
    }
    .info_stats{
      padding: 10px;
    }
    .info_stats > h5{
      text-align: center;
    }
    .count{
      padding: 0;
      margin: 0;
      font-size: 50px;
      font-weight: 600;
    }

    @media screen and  (max-width: 468px) {
      .container{
        width: 100%;
        display: inline-block;
      }
      .left_side{
        width: 100%;
        position: relative;
      }

      .right_side{
        width: 100%;
        position: relative;
      }
    }


</style>
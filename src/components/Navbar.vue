<template>
  <div class="container">
    <nav class="navbar navbar-expand-lg">
      <div class="container col-12">
        <a href="#" class="navbar-brand d-flex">
          <img src="../assets/LogoGroup.svg" alt="">
          <p class="logoBrand">TheBox</p>
        </a>
        <div class="nav">
          <ul class="navbar-nav">
            <li class="nav-item">
                Home
            </li>
            <li class="nav-item">
                About Us
            </li>
            <li class="nav-item">
                Projects
            </li>
            <li class="nav-item">
                Services
            </li>
            <li class="nav-item active">
                Contact Us
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
// import LogoImg from '/assets/LogoGroup.svg'
export default {
  name: "Nav-bar",
}
</script>

<style scoped>
  .active{
    color: #f9995D;
  }
  .navbar-nav{
    margin-left: auto;
  }
  .navbar-brand{
    text-align: center;
    justify-content: center;
  }
  .nav-item{
    font-size: 18px;
    margin-right: 50px;
    transition: 200ms ease-in;
    font-family: 'Work Sans';
  }
  .nav-item:hover{
    transition: 150ms ease-in;
    color: #f9995D;
    cursor: pointer;
  }
  .logoBrand{
    margin-top: 12px;
    font-style: italic;
    font-weight: 700;
    font-size: 30px;
    line-height: 35px;
    color: #2947A9;
  }
  @media screen and (min-width: 480px) {
    .navbar-nav{
      display: none;
    }
  }

  @media screen and (min-width: 768px) {
    .navbar-nav{
      display: inline-block;
    }
  }

  @media screen and (min-width: 1024px) {
    .navbar-nav{
      display: flex;
    }
  }

</style>
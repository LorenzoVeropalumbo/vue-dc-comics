<template>
  <footer>
    <div class="container">
      <div class="footer-top">
        <ul>
          <li class="ul-section">DC COMICS</li>
          <li><a href="#">Character</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">News</a></li>
          <li class="ul-section">SHOP</li>
          <li><a href="#">Shop DC</a></li>
          <li><a href="#">Shop DC Collectibles</a></li>
        </ul>
        <ul>
          <li class="ul-section">DC</li>
          <li><a href="#">Terms Of Us</a>e</li>
          <li><a href="#">Privacy polict(New)</a></li>
          <li><a href="#">Ad Choise</a></li>
          <li><a href="#">Advertaising</a></li>
          <li><a href="#">Jobs</a></li>
          <li><a href="#">Subscription</a></li>
          <li><a href="#">Talent Workshops</a></li>
          <li><a href="#">CPSC Certificates</a></li>
          <li><a href="#">Ratings</a></li>
          <li><a href="#">Shop Help</a></li>
          <li><a href="#">Contact Us</a></li>
        </ul>
        <ul>
          <li class="ul-section">SITES</li>
          <li><a href="#">DC</a></li>
          <li><a href="#">MAD Magazine</a></li>
          <li><a href="#">DC Kids</a></li>
          <li><a href="#">DC Universe</a></li>
          <li><a href="#">DC Power Visa</a></li>
        </ul>
      </div>
      <div class="bg-img">
      </div>
         
    </div>
  </footer>
</template>

<script>
  export default {
    name: "DcFooterComp"
  }
</script>

<style lang="scss" scoped>
  footer{   
    background-image: url(../assets/footer-bg.jpg);
    background-size: cover;
    color: #949494;
    font-size: 12px;
    .container{
      display: flex;
      justify-content: space-between;
      
      .footer-top{    
        
        padding: 40px 0 0;
        margin: 0 20px;
        position: relative;
        z-index: 1;
        width: 30%;
        display: flex;
        justify-content: space-between;

        li{
          padding: 3px 0;
        }
  
        .ul-section{
          color: white;
          font-size: 21px;
          font-weight: 700;
          padding: 10px 0;
        }

        
      }
      div.bg-img{
        height: 370px;
        width: 560px;
        background-image: url(../assets/dc-logo-bg.png);
        background-size: cover;
        background-position: center;
        
      }      
    }
  }

</style>
<template>
  <footer>
    <nav class="d_flex_between container">
      <!-- image logo -->
      <span class="btn">SIGN-UP NOW!</span>  
        <!-- Nav ul -->
      <ul>
        <li class="text">FOLLOW US</li>
        <li><img src="../assets/footer-facebook.png" alt=""></li>
        <li><img src="../assets/footer-twitter.png" alt=""></li>
        <li><img src="../assets/footer-youtube.png" alt=""></li>
        <li><img src="../assets/footer-pinterest.png" alt=""></li>
        <li><img src="../assets/footer-periscope.png" alt=""></li>
      </ul>
    </nav>
  </footer>
</template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>
  footer{
    background-color: #303030;
    padding: 30px 0;

    .btn{
      border: 2px solid #0082f9;
      padding: 15px;
      color: white;
      font-weight: 600;
      font-size: 16px;
    }

    ul{
      display: flex;
      align-items: center;
      .text{
        font-size: 21px;
        font-weight: 900;
        color: #0082f9;
      }
      li{
        padding: 0 10px;
        img{
          width: 35px;
          height: 35px;
        } 
      }
      
    }

  }
</style>
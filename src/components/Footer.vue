<template>
  <footer>
    <div class="footer-top">
      <div class="wrapper-footer container">

        <nav class="left">
          <ul>
            <h3>dc comics</h3>
            <li v-for="(dcComic,index) in dcComics" :key="index">
              <a :href="dcComic.url">{{dcComic.text}}</a>
            </li>
            <!-- <li><a href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">News</a></li> -->
          </ul>
          <ul>
            <h3>shops</h3>
            <li v-for="(shop,index) in shops" :key="index">
              <a :href="shop.url">{{shop.text}}</a>
            </li>
            <!-- <li><a href="#">Shop DC collectibles</a></li> -->
          </ul>
        </nav>
        <nav class="left">
          <ul>
            <h3>dc</h3>
            <li v-for="(dc,index) in dcS" :key="index">
              <a :href="dc.url">{{dc.text}}</a>
            </li>
            <!-- <li><a href="#">Privacy policy (New)</a></li>
            <li><a href="#">Ad Choices</a></li>
            <li><a href="#">Advertising</a></li>
            <li><a href="#">Jobs</a></li>
            <li><a href="#">Subscriptions</a></li>
            <li><a href="#">Talent Workshops</a></li>
            <li><a href="#">CPSC Certificates</a></li>
            <li><a href="#">Ratings</a></li>
            <li><a href="#">Shop Help</a></li>
            <li><a href="#">Contact Us</a></li> -->
          </ul>
        </nav>
        <nav class="left">
          <ul>
            <h3>sites</h3>
            <li v-for="(site,index) in sites" :key="index">
              <a :href="site.url">{{site.text}}</a>
            </li>
            <!-- <li><a href="#">MAD Magazine</a></li>
            <li><a href="#">DC Kinds</a></li>
            <li><a href="#">DC Universe</a></li>
            <li><a href="#">DC Power Visa</a></li> -->
          </ul>
        </nav>

      </div>
      
    </div>

    <div class="footer-bottom">
    <div class="bottom container">
      <a id="btn" href="#">Sign-up now!</a>

      <div class="social-list">
        <ul>
          <h3>Follow us</h3> 
          <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="Facebook"></a></li>
          <li><a href="#"><img src="../assets/img/footer-twitter.png" alt="Twitter"></a></li>
          <li><a href="#"><img src="../assets/img/footer-youtube.png" alt="YouTube"></a></li>
          <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt="Pinterest"></a></li>
          <li><a href="#"><img src="../assets/img/footer-periscope.png" alt="Periscope"></a></li>
        </ul>
      </div>
    </div>
    </div>

  </footer>
</template>

<script>

export default {
  name: 'Footer',
  data(){
    return{
      dcComics:[
        {
        text:'Characters',
        url:'#'
        },
        {
        text:'Comics',
        url:'#'
        },
        {
        text:'Movies',
        url:'#'
        },
        {
        text:'TV',
        url:'#'
        },
        {
        text:'Games',
        url:'#'
        },
        {
        text:'Videos',
        url:'#'
        },
        {
        text:'News',
        url:'#'
        },
      ],

      shops:[
        {
          text:'Shop DC',
          url:'#'
        },
        {
          text:'Shop DC collectibles',
          url:'#'
        },
      ],

      dcS:[
        {
        text:'Terms Of Use',
        url:'#'
        },
        {
        text:'Privacy policy (New)',
        url:'#'
        },
        {
        text:'Ad Choices',
        url:'#'
        },
        {
        text:'Advertising',
        url:'#'
        },
        {
        text:'Jobs',
        url:'#'
        },
        {
        text:'Subscriptions',
        url:'#'
        },
        {
        text:'Talent Workshops',
        url:'#'
        },
        {
        text:'CPSC Certificates',
        url:'#'
        },
        {
        text:'Ratings',
        url:'#'
        },
        {
        text:'Shop Help',
        url:'#'
        },
        {
        text:'Contact Us',
        url:'#'
        },
      ],
      sites: [
        {
          text: 'DC',
          url: '#'
        },
        {
          text: 'MAD Magazine',
          url: '#'
        },
        {
          text: 'DC Kinds',
          url: '#'
        },
        {
          text: 'DC Universe',
          url: '#'
        },
        {
          text: 'DC Power Visa',
          url: '#'
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>

  @import '../assets/style/vars.scss';

  .footer-top{
    background-image: url(../assets/img/footer-bg.jpg);
    height: 370px;
    background-size: cover;
  }
  .wrapper-footer{
    background-image: url(../assets/img/dc-logo-bg.png);
    height: 100%;
    background-repeat: no-repeat;
    background-position: 98% 50%;
    background-size: 43%;
    padding:  30px 0;
    nav{
      margin-right: 25px;

      h3{
        color: white;
        font-weight: 400;
        text-transform: uppercase;
        margin: 10px 0;
      }
      li{
        padding: 1px 0;
        a{
          font-size: 13px;
          color: #959595;
        }
      }
    }
  }
  
  .footer-bottom{
    background-color: #303030;
  }

  .bottom {
    height: 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;

    h3{
      color: $colorBrand;
      text-transform: uppercase;
    }
    
    #btn {
      display: inline-block;
      color: white;
      text-decoration: none;
      text-transform: uppercase;
      padding: 10px;
      font-weight: 600;
      border: 2px solid $colorBrand;
      &:hover {
        transform: scale(1.1);
      }
    }
    ul {
      
      display: flex;
      align-items: center;

      li {
        margin-left: 20px;
        
        img {
          height: 30px;
        }
      }
    }
  }
</style>
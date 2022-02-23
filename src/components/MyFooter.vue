<template>
  <footer>
    <div class="footer-top">
      <div class="list">
        <h3>DC COMICS</h3>
        <MyList 
          v-for="(el, index) in dcComics"
          :key="index"
          :element='el'>
        </MyList>
      </div>

      <div class="list">
        <h3>SHOP</h3>
        <MyList 
          v-for="(el, index) in shop"
          :key="index"
          :element='el'>
        </MyList>
      </div>

      <div class="list">
        <h3>DC</h3>
        <MyList 
          v-for="(el, index) in dc"
          :key="index"
          :element='el'>
        </MyList>
      </div>
      
      <div class="list">
        <h3>SITES</h3>
        <MyList 
          v-for="(el, index) in sites"
          :key="index"
          :element='el'>
        </MyList>
      </div>
      <img src="../assets/img/dc-logo-bg.png">
    </div>
    <div class="footer-bottom">
      <div class="btn">SIGN-UP NOW!</div>
      <div class="social">
        <span>FOLLOW US</span>
        <ul>
          <li><img src="../assets/img/footer-facebook.png" alt=""></li>
          <li><img src="../assets/img/footer-twitter.png" alt=""></li>
          <li><img src="../assets/img/footer-youtube.png" alt=""></li>
          <li><img src="../assets/img/footer-pinterest.png" alt=""></li>
          <li><img src="../assets/img/footer-periscope.png" alt=""></li>
        </ul>
      </div>
    </div>
    
  
  </footer>
</template>

<script>
import MyList from './MyList.vue';

export default {
  name: 'MyFooter',
  components: {
    MyList
  },
  data() {
    return {
      dcComics: [
        {
          text: 'Characters'
        },
        {
          text: 'Comics'
        },
        {
          text: 'Movies'
        },
        {
          text: 'TV'
        },
        {
          text: 'Games'
        },
        {
          text: 'Videos'
        },
        {
          text: 'News'
        }
      ],
      shop: [
        {
          text: 'Shop DC'
        },
        {
          text: 'Shop DC Collectibles'
        }
      ],
      dc: [
        {
          text: 'Terms Of Use'
        },
        {
          text: 'Privacy Policy (New)'
        },
        {
          text: 'Ad Choices'
        },
        {
          text: 'Advertising'
        },
        {
          text: 'Jobs'
        },
        {
          text: 'Subscriptions'
        },
        {
          text: 'Talent Workshops'
        },
        {
          text: 'CPSC Certificates'
        },
        {
          text: 'Ratings'
        },
        {
          text: 'Shop Help'
        },
        {
          text: 'Contact Us'
        }
      ],
      sites: [
        {
          text: 'DC'
        },
        {
          text: 'MAD Magazine'
        },
        {
          text: 'DC Kids'
        },
        {
          text: 'DC Universe'
        },
        {
          text: 'DC Power Visa'
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .footer-top {
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    padding: 20px 15%;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    height: 380px;
    align-content: flex-start;
    position: relative;

    img {
      position: absolute;
      top: 50%;
      right: 20px;
      transform: translate(0,-50%);
    }
    
    .list {
      width: fit-content;
    }

    h3 {
    color: white;
    margin: 15px;
    }
  }

  .footer-bottom {
    padding: 20px 15%;
    height: 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: rgb(39, 39, 39);
    position: relative;
    z-index: 10;

    .btn {
      
      padding: 10px;
      border: 1px solid rgb(17, 100, 255);
      color: white;
      font-weight: bold;
      height: fit-content;

      &:hover {
        cursor: pointer;
      }
    }
    
    .social {
      display: flex;
      align-items: center;
      color: rgb(17, 100, 255);
      font-weight: bold;
      
      span {
        margin-right: 10px;
      }

      li {
        display: inline-block;
        list-style: none;
        margin: 0 5px;
        &:hover {
          cursor: pointer;
        }
      }
    }
  }
  
</style>

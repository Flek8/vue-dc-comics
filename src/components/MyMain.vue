<template>
  <main>
      <MyJumbotron/>
      <div id="merchandise">
          <ul>
              <li v-for="(product, index) in products" :key="index">
                  <img :src="product.photo">
                  {{product.text}}
              </li>
          </ul>
      </div>
  </main>
</template>

<script>
import MyJumbotron from './MyJumbotron.vue'

export default {
  name: 'MyMain',
  components: {
      MyJumbotron
  },
  data() {
      return {
          products: [
              {
                  text: 'DIGITAL COMICS',
                  photo: require('../assets/img/buy-comics-digital-comics.png')
              },
              {
                  text: 'DC MERCHANDISE',
                  photo: require('../assets/img/buy-comics-merchandise.png')
              },
              {
                  text: 'SUBSCRIPTION',
                  photo: require('../assets/img/buy-comics-subscriptions.png')
              },
              {
                  text: 'COMIC SHOP LOCATOR',
                  photo: require('../assets/img/buy-comics-shop-locator.png')
              },
              {
                  text: 'DC POWER VISA',
                  photo: require('../assets/img/buy-dc-power-visa.svg')
              }
          ]
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    main {
        background-color: rgb(17, 100, 255);
    }
    
    #merchandise {
        width: 70%;
        margin: auto;
        background-color: rgb(17, 100, 255);
        padding: 30px 0;

        ul {
            height: 100%;
            display: flex;
            flex-direction: row;
            justify-content: space-around;
            align-items: center;
            li {
                color: white;
                list-style-type: none;
                font-size: 10px;
                display: flex;
                align-items: center;
                img {
                    height: 50px;
                    width: 50px;
                    object-fit: contain;
                    margin-right: 5px;
                    &:hover {
                        cursor: pointer;
                    }
                }
            }
        }
    }
</style>

<template>
  <main>
      <div id="jumbotron">
          <div id="content">
              <h1>Content goes here</h1>
          </div>
      </div>

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
export default {
  name: 'MyMain',
  data() {
      return {
          products: [
              {
                  text: 'DIGITAL COMICS',
                  photo: '../assets/img/buy-comics-digital-comics.png'
              },
              {
                  text: 'DC MERCHANDISE',
                  photo: '../assets/img/buy-comics-merchandise.png'
              },
              {
                  text: 'SUBSCRIPTION',
                  photo: '../assets/img/buy-comics-shop-locator.png'
              },
              {
                  text: 'COMIC SHOP LOCATOR',
                  photo: '../assets/img/buy-comics-subscriptions.png'
              },
              {
                  text: 'DC POWER VISA',
                  photo: '../assets/img/buy-dc-power-visa.svg'
              }
          ]
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    #jumbotron {
        background-color: black;
        #content {
            width: 70%;
            margin: auto;
            height: 100px;
            line-height: 100px;
            color: white;
            vertical-align: middle;
        }
    }
    #merchandise {
        background-color: rgb(17, 100, 255);
        height: 150px;

        ul {
            height: 100%;
            display: flex;
            flex-direction: row;
            justify-content: space-around;
            align-items: center;
            li {
                color: white;
                list-style-type: none;
                img {
                    height: 30px;
                }
            }
        }
    }
</style>

<template>
  <header>
      <img src="../assets/img/dc-logo.png" height="70" alt="dc logo">
      <div>
          <ul>
              <li v-for="(link, index) in links" :key="index">
                  <a :href="link.url">{{link.text}}</a>
              </li>
          </ul>
      </div>
  </header>
</template>

<script>
export default {
  name: 'MyHeader',
  data() {
      return {
          links: [
          {
              text: 'CHARACTERS',
              url: '#',
              active: false
          },
           {
              text: 'COMICS',
              url: '#',
              active: false
          },
           {
              text: 'MOVIES',
              url: '#',
              active: false
          },
           {
              text: 'TV',
              url: '#',
              active: false
          },
           {
              text: 'GAMES',
              url: '#',
              active: false
          },
           {
              text: 'COLLECTIBLES',
              url: '#',
              active: false
          },
           {
              text: 'VIDEOS',
              url: '#',
              active: false
          },
           {
              text: 'FANS',
              url: '#',
              active: false
          },
           {
              text: 'NEWS',
              url: '#',
              active: false
          },
           {
              text: 'SHOP',
              url: '#',
              active: false
          },
          ]
        }
      
    }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    header {
        width: 70%;
        margin: auto;
        height: 100px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        
        ul {
            height: 100px;
            display: flex;
            align-items: center;
            li{
                display: inline;
                line-height: 100px;
                vertical-align: middle;
                height: 100%;
                margin: 10px;
                font-size: 12px;
                &:hover {
                    border-bottom: 4px solid rgb(17, 100, 255);
                }
                &:hover a {
                    color: rgb(17, 100, 255);
                }
                a {
                    font-weight: bold;
                    text-decoration: none;
                    color: black;
                }
            }
        }
    }
</style>
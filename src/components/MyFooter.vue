<template>
  <div>
    <MyList msg="dcComics"/>
  </div>
</template>

<script>
import MyList from './MyList.vue'

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

</style>

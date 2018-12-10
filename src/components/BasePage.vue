<template>
  <b-container
    fluid
  >
    <header id="page1">
      <b-container class="h-100 toppage">
        <b-row align-v="center">
          <b-col md="7">
            <b-img
              fluid
              src='../logo2.png'
            />
            <h1>Beer discoveries at your fingertips</h1>

            <p>Beer Peer informs and helps you discover new craft beer across the
              nation without the need to travel. Browse, swipe, and order beers right
              to your doorstep.</p>

            <ul>
              <li>Find new beer with personalized recomendations</li>
              <li>Order beers from new breweries</li>
              <li>Share your discoveries with all your friends</li>
            </ul>

            <b-button variant='primary' @click='download'>
              Download Now&#32;&#32;

              <font-awesome-icon icon='download' />
            </b-button><br />
            <strong>*Button will not download</strong>

          </b-col>

          <b-col md="5">
            <b-img
              fluid
              class='iphone'
              src="../3iphones.png"
            />
          </b-col>
        </b-row>
      </b-container>

    </header>

      <b-container id="page2" class="second">
        <b-row>
          <h1>Discover Beer Peer!</h1>
        </b-row>
        <b-row>
          <b-col md="4">
            <b-img
              fluid
              src="../iPhoneDetails.png"
            />

            <p>
              <strong>Discover Beers</strong><br />
               View detailed information on different beers to find brews to try!

            </p>
          </b-col>

          <b-col md="4">
            <b-img
              fluid
              src="../iPhoneRecomend.png"
            />


            <p>
              <strong>Receive Recomendations</strong><br />
               Beer Peer's powerful personal recomendation engine will ensure you find brews that you love!

            </p>
          </b-col>

          <b-col md="4">
            <b-img
              fluid
              src="../iPhoneOrder.png"
            />


          <p>
            <strong>Order to Your Doorstep</strong><br />
             If you can't find a beer locally, simply order it through Beer Peer!

          </p>
          </b-col>
        </b-row>
        <b-row>
          <b-button variant='primary' @click='download'>
            Download Now&#32;&#32;

            <font-awesome-icon icon='download' />
          </b-button>
        </b-row>
        <b-row>
            <strong>*Button will not download</strong>
        </b-row>
      </b-container>


  </b-container>
</template>


<script>
import bContainer from 'bootstrap-vue/es/components/layout/container'
import bCol from 'bootstrap-vue/es/components/layout/col'
import bRow from 'bootstrap-vue/es/components/layout/row'
import bButton from 'bootstrap-vue/es/components/button/button'
import bImg from 'bootstrap-vue/es/components/image/img'


export default {
  name: 'BasePage',
  props: {
    msg: String
  },
  components: {
    'b-container': bContainer,
    'b-col': bCol,
    'b-row': bRow,
    'b-button': bButton,
    'b-img': bImg
  },
  methods: {
    download: function(){
      window.location.href = 'http://bit.ly/2PGVwRI'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.toppage{
  padding-top: 7%;
  padding-bottom: 8%;
}

#page2{
  padding-bottom: 30px;
}

.floating-button{
  position: fixed;
  bottom: 30px;
  right: 30px;
  cursor: pointer;
}


</style>

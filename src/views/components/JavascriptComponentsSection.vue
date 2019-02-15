<template>
  <div class="wrapper">
    <div id="javascriptComponents">
      <div class="md-layout">
        <div class="md-layout-item md-small-size-100">
          <md-card>
            <carousel
                    :per-page="1"
                    loop
                    :speed="700"
                    autoplay
                    :autoplay-timeout="5000"
                    :mouse-drag="false"
                    navigationEnabled
                    navigationNextLabel="<i class='material-icons'>keyboard_arrow_right</i>"
                    navigationPrevLabel="<i class='material-icons'>keyboard_arrow_left</i>"
            >
              <slide>
                <div class="carousel-caption">
                  <h4>
                    <md-icon>location_on</md-icon>
                    Beyond your widest Dreams
                  </h4>
                </div>
                <img :src="carousel1" alt="carousel1" />
              </slide>
              <slide>
                <div class="carousel-caption">
                  <h4>
                    <md-icon>location_on</md-icon>
                    Lets Build this
                  </h4>
                </div>
                <img :src="carousel2" alt="carousel2" />
              </slide>
              <slide>
                <div class="carousel-caption">
                  <h4>
                    <md-icon>location_on</md-icon>
                    Yes I can
                  </h4>
                </div>
                <img :src="carousel3" alt="carousel3" />
              </slide>
            </carousel>
          </md-card>
        </div>
        <div class="md-layout-item md-small-size-100 md-alignment-top-space-around md-alignment-center-center md-alignment-bottom-center">
          <div class="title">
            <h1 class="text-center strong">Headlines</h1>
          </div>
          <div class="md-layout">
            <div class="md-layout-item">

              <h4 class="text-center">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
                laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate
                velit esse cillum dolore eu fugiat.!</h4>

               <div class="text-center"> <md-button class="md-success" >On right</md-button> </div>
            </div>
          </div>

        </div>
      </div>

    </div>
  </div>
</template>

<script>
import { Modal } from "@/components";
export default {
  components: {
    Modal
  },
  data() {
    return {
      classicModal: false,
      selectedDate: new Date("2018/03/26"),
      carousel1: require("@/assets/img/nature-2.jpg"),
      carousel2: require("@/assets/img/nature.jpg"),
      carousel3: require("@/assets/img/nature-3.jpg")
    };
  },
  methods: {
    classicModalHide() {
      this.classicModal = false;
    }
  }
};
</script>

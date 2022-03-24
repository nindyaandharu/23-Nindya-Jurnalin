<template>
<v-app>
  <v-card color="#66806A">
    <v-card-title class="text-center justify-center py-6">
      <h1 class="font-weight-bold text-h2 white--text">
        JURNALIN
      </h1>
    </v-card-title>

    <v-tabs
      v-model="tab"
      background-color="transparent"
      color="white"
      grow
    >
      <v-tab
        v-for="item in items"
        :key="item"
      >
        {{ item }}
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item
        v-for="item in items"
        :key="item"
      >
        <v-card
          color="basil"
          flat
        >
          
        </v-card>
      </v-tab-item>
    </v-tabs-items>
  </v-card>

  <!-- Sizes your content based upon application components -->
  <v-main>

    <!-- Provides the application the proper gutter -->
    
      <!-- <div id="app">
        <img src="./assets/Rectangle 7.png" alt="Vue Book">
      </div> -->
      <v-row>
      <v-col> 
        <v-img src="./assets/Rectangle 7.png" width="1000" height="600" class="mt-10" position= "relative"> </v-img>
      </v-col>
      <v-col align-self="center">
        <H3 class="text-hello">
          HAI, NINDYA! SAVE YOUR MEMORIES FOR TODAY!</H3>
      </v-col>
      </v-row>
      <v-card-text class="text-choose mt-5" align="center">choose according to your needs</v-card-text>

    <v-container class="mt-5 mb-15">
    <v-row>
      <v-col cols="4"> <v-img src="./assets/Ellipse 2.png"></v-img> </v-col>
      <v-col cols="6" class="text-diary" align-self="center"> 
        <h3>DIARY</h3> 
        <p>You can reminisce all memories to keep them in mind</p>
      </v-col>
      <v-col align-self="center"> 
        <v-btn
        outlined
        color="#66806A"
        width="120"
        height="45">
        CREATE
        </v-btn>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="4"> <v-img src="./assets/Ellipse 4.png"></v-img> </v-col>
      <v-col cols="6" class="text-Calender" align-self="center"> 
        <h3>CALENDER MOOD</h3> 
        <p>Record details of your mood every day</p>
      </v-col>
      <v-col align-self="center"> 
        <v-btn
        outlined
        color="#66806A"
        width="120"
        height="45">
        CREATE
        </v-btn>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="4"> <v-img src="./assets/Ellipse 5.png"></v-img> </v-col>
      <v-col cols="6" class="text-Todo" align-self="center"> 
        <h3>TO DO</h3> 
        <p>Write down what you want to do so you don't miss it</p>
      </v-col>
      <v-col align-self="center"> 
        <v-btn
        outlined
        color="#66806A"
        width="120"
        height="45">
        CREATE
        </v-btn>
      </v-col>
    </v-row>
  </v-container>

  <v-img src="./assets/Rectangle 8.png" class="mt-15" height="670">
  <v-container>
    <v-card-text class="text-TESTI text-center justify-center white--text">
      TESTIMONIALS
    </v-card-text>
  <v-row>
    <v-col>
      <v-card
        class="mx-auto"
        color="#E1C892"
        dark
        max-width="400">
    <v-card-actions>
      <v-list-item class="grow">
        <v-list-item-avatar color="grey darken-3">
          <v-img
            class="elevation-6"
            alt=""
            src="https://i.pinimg.com/564x/52/4a/ae/524aae7a21f2014b4e6005551f83e704.jpg"
          ></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title class="text-h5">Elmeira Navari</v-list-item-title>
          <v-rating
          :value="4.5"
          color="white"
          dense
          half-increments
          readonly
          size="14"
        ></v-rating>
        </v-list-item-content>
      </v-list-item>
    </v-card-actions>
    <v-card-text class="text-h5 font-weight-bold">
      "finally i found this website, I like to take notes on a mood calendar, and now I don't need to use books anymore."
    </v-card-text>  
      </v-card>
    </v-col>
    <v-col>
      <v-card
        class="mx-auto"
        color="#E1C892"
        dark
        max-width="400">
    <v-card-actions>
      <v-list-item class="grow">
        <v-list-item-avatar color="grey darken-3">
          <v-img
            class="elevation-6"
            alt=""
            src="https://i.pinimg.com/564x/c2/cc/9f/c2cc9f200b765e4abec893f54dc9afd3.jpg">
          </v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title class="text-h5">Erisha Danurdara</v-list-item-title>
          <v-rating
          :value="5.0"
          color="white"
          dense
          half-increments
          readonly
          size="14"
        ></v-rating>
        </v-list-item-content>
      </v-list-item>
    </v-card-actions>
    <v-card-text class="text-h5 font-weight-bold">
      "for me, this is a brilliant idea. I am very comfortable and enjoy using JURNALIN. Thank you for made this website"
    </v-card-text>  
    </v-card>
    </v-col>
    <v-col>
      <v-card
        class="mx-auto"
        color="#E1C892"
        dark
        max-width="400">
    <v-card-actions>
      <v-list-item class="grow">
        <v-list-item-avatar color="grey darken-3">
          <v-img
            class="elevation-6"
            alt=""
            src="https://i.pinimg.com/564x/56/dc/9f/56dc9f45292a60f48243bbe64df4b6aa.jpg">
          </v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title class="text-h5">Abel Khaizure</v-list-item-title>
          <v-rating
          :value="4.0"
          color="white"
          dense
          half-increments
          readonly
          size="14"
        ></v-rating>
        </v-list-item-content>
      </v-list-item>
    </v-card-actions>
    <v-card-text class="text-h5 font-weight-bold">
      "Sangat baik dan berguna untuk sehari-hari, hanya saja desain terlalu besar. So far so good."
    </v-card-text>  
    </v-card>
    </v-col>
  </v-row>

  <center>
    <v-card-text class="text-RATE white--text mt-10">
      TAP TO RATE
    </v-card-text>
  
    <v-rating
      v-model="rating"
      background-color="white lighten-3"
      color="white"
      large
    ></v-rating>
    <v-row justify="center">
      <v-col class="mt-5" cols="9" md="3">
        <v-text-field
            label="Write a review"
            outlined
            width="200px"
            height="100px"
            color="white"
          ></v-text-field>
      </v-col>
    </v-row>
      <v-btn
        outlined
        color="white"
      >
      SUBMIT
    </v-btn>
  </center>
  </v-container>
  </v-img>
      <!-- If using vue-router -->
      <router-view></router-view>
  </v-main>

  <v-footer
    dark
    padless
  >
    <v-card
      flat
      tile
      class="white--text text-center"
      color="#E1C892"
    >
      <v-card-text>
        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4 white--text"
          icon
        >
         
        </v-btn>
      </v-card-text>

      <v-card-text class="text-foot white--text pt-0">
        We created this website to make it easier for us to organize all the precious moments in life, 
        So that they are always remembered.
        And of course we also accept criticism and suggestions which if you take the time to fill it out, 
        we really appreciate it. Thank you
      </v-card-text>

      <v-divider></v-divider>

      <v-card-text class="white--text">
        {{ new Date().getFullYear() }} — <strong>JURNALIN</strong>
      </v-card-text>
    </v-card>
  </v-footer>
</v-app>
</template>

<script>
export default {
  data: () => {
    return {
        tab: null,
        items: [
          'HOME', 'DIARY', 'CALENDER MOOD', 'TO DO','ABOUT US'
        ],
      }
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Asap&display=swap');
.text-choose{
  font-family: 'Asap';
  font-size: 30px !important;
  font-style: italic;
}
.text-hello{
  font-family: 'Asap';
  font-size: 70px;
  line-height: 80px;
  font-weight: 600;
  width: 370px;
}
.text-diary{
  font-family: 'Asap';
  font-size: 36px;
}
.text-Calender{
  font-family: 'Asap';
  font-size: 36px;
}
.text-Todo{
  font-family: 'Asap';
  font-size: 36px;
}
.text-TESTI{
  font-family: 'Asap';
  font-size: 24px !important;
  font-style: italic;
}
.text-RATE{
  font-family: 'Asap';
  font-size: 24px !important;
  font-style: italic;
}
.text-foot{
  font-family: 'Asap';
  font-size: 24px !important;
}
</style>
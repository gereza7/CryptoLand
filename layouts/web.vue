<template>
  <div>
    <div
   
    >
      <div style="height: 20px; padding: 0px; margin-bottom: 15px; width: 100%; margin-top:-8px">
        <iframe
          src="https://widget.coinlib.io/widget?type=horizontal_v2&theme=light&pref_coin_id=1505&invert_hover="
          width="100%"
          height="36px"
          scrolling="auto"
          marginwidth="0"
          marginheight="0"
          frameborder="0"
          border="0"
          style="border: 0; margin: 0; padding: 0"
        ></iframe>
      </div>
     
    </div>

    <v-app-bar color="#7C4DFF" dense dark style="height: 75px">
      <v-img
        lazy-src="https://i.ibb.co/rbh95FW/Crypto-Land-Logo.png"
        max-height="100"
        max-width="250"
        src="https://i.ibb.co/rbh95FW/Crypto-Land-Logo.png"
        style="align: center"
      ></v-img>

      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>

      <v-menu left bottom>
        <template v-slot:activator="{ on, attrs }">
          <v-btn icon v-bind="attrs" v-on="on">
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
        </template>

        <v-list>
          <v-list-item v-for="n in 5" :key="n" @click="() => {}">
            <v-list-item-title>Option {{ n }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
    </v-app-bar>
    <Nuxt />
  </div>
</template>

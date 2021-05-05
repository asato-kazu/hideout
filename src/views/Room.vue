<template>
  <v-app>
    <v-main>
  <div class="room">
    <v-container style="width: 600px;">
      <h1>Room</h1>
    </v-container>
     <v-card class="mt-4 mb-4 pa-3">
            <v-layout row wrap>
                <v-flex xs4 v-for="(item,i) in items" :key="i"> 
                    <v-card class="grey lighten-3 ma-2">
                        <v-card-text><img v-bind:src="item.src" width="100%" alt=""></v-card-text>
                    </v-card>
                </v-flex>
            </v-layout>
      </v-card>
  </div>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: 'Room',
  data: () => ({
    items: [
                {src: "/img/hideout.jpg"},
                {src: "/img/hideout.jpg"},
                
            ]
  })
}
</script>

<template>
    <v-navigation-drawer permanent class="float-left">
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="title">
            Hotel Hide Out
          </v-list-item-title>
          <v-list-item-subtitle>
            subtext
          </v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>

      <v-list
        dense
        nav
      >
        <v-list-item link @click="goHome()">
            <v-list-item-icon>
                <v-icon>mdi-view-dashboard</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
                <v-list-item-title>Home</v-list-item-title>
            </v-list-item-content>
        </v-list-item>

        <v-list-item link @click="goRoom()">
            <v-list-item-icon>
                <v-icon>mdi-view-dashboard</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
                <v-list-item-title>Room</v-list-item-title>
            </v-list-item-content>
        </v-list-item>

        <v-list-item link @click="goRes()">
            <v-list-item-icon>
                <v-icon>mdi-image</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
                <v-list-item-title>Reservation</v-list-item-title>
            </v-list-item-content>
        </v-list-item>

        <v-list-item link @click="goAcc()">
            <v-list-item-icon>
                <v-icon>mdi-image</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
                <v-list-item-title>Access</v-list-item-title>
            </v-list-item-content>
        </v-list-item>

        <v-list-item link @click="goCont()">
            <v-list-item-icon>
                <v-icon>mdi-image</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
                <v-list-item-title>Contact</v-list-item-title>
            </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
</template>

<script>
export default {
  name: 'Navi',

  data: () => ({
    items: [
      { title: 'Test', icon: 'mdi-help-box' },
    ],
    right: null,
  }),

  methods: {
      goHome: function () {
          this.$router.push('/');
      },
      goRoom: function () {
          this.$router.push('/room');
      },
      goRes: function () {
          this.$router.push('/reservation');
      },
      goAcc: function () {
          this.$router.push('/access');
      },
      goCont: function () {
          this.$router.push('/contact');
      },
  }
}
</script>
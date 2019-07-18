<template>
  <v-app dark>
    <default-header />
  </v-app>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import DefaultHeader from "~/components/layout/header.vue";

@Component({
  components: {
    DefaultHeader
  }
})
export default class Tmp extends Vue {
  clipped: boolean = false;
  drawer: boolean = false;
  fixed: boolean = false;
  items: { [key: string]: string }[] = [
    {
      icon: "apps",
      title: "Welcome",
      to: "/"
    },
    {
      icon: "bubble_chart",
      title: "Inspire",
      to: "/inspire"
    }
  ];
  miniVariant: boolean = false;
  right: boolean = true;
  rightDrawer: boolean = false;
  title: string = "Vuetify.js";
  //data() {
  //  return {
  //    clipped: false,
  //    drawer: false,
  //    fixed: false,
  //    items: [
  //      {
  //        icon: 'apps',
  //        title: 'Welcome',
  //        to: '/'
  //      },
  //      {
  //        icon: 'bubble_chart',
  //        title: 'Inspire',
  //        to: '/inspire'
  //      }
  //    ],
  //    miniVariant: false,
  //    right: true,
  //    rightDrawer: false,
  //    title: 'Vuetify.js'
  //  }
  //}
}
</script>

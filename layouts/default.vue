<template>

    <v-main>
      <!-- <TheHeader @sidenavToggle = "displaySidenav=!displaySidenav"/>

      <TheSidenav :show="displaySidenav"
      @close="displaySidenav"/> -->
      <TheHeader/>
      <TheSidenav/>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>

   
</template>

<script>
import TheHeader from '../components/Navigation/TheHeader.vue'
import TheSidenav from '../components/Navigation/TheSidenav.vue'
// import TheSideNavToggle from '../components/Navigation/TheSideNavToggle.vue'
export default {
  name: 'DefaultLayout',
  components:{
    TheHeader,
    TheSidenav,
  //   TheSideNavToggle
  },
  data(){
     return{
     displaySidenav:false
     }
  },
  // data () {
  //   return {

  //     clipped: false,
  //     drawer: false,
  //     fixed: false,
  //     items: [
  //       {
  //         icon: 'mdi-apps',
  //         title: 'Welcome',
  //         to: '/'
  //       },
  //       {
  //         icon: 'mdi-chart-bubble',
  //         title: 'Inspire',
  //         to: '/inspire'
  //       }
  //     ],
  //     miniVariant: false,
  //     right: true,
  //     rightDrawer: false,
  //     title: 'Vuetify.js'
  //   }
  // }
}
</script>
 <!-- <TheHeader @SidenavToggle="displaySidenav=!displaySidenav"/>
      <TheSidenav
      :show="displaySidenav"
      @close="displaySidenav=false"/> -->
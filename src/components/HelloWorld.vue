<template>
<ion-app>
   <ion-header>
        <ion-toolbar color="primary">
          <ion-title>Cardio Challenges </ion-title>
        </ion-toolbar>
      </ion-header>
<ion-content padding>
 <ion-searchbar></ion-searchbar>
       <ion-list>
    <ion-item>
      <ion-range min="1" max="3" step="1" snaps="true" color="secondary">
        <ion-label slot="start">Beginner</ion-label>
        <ion-label slot="end">Advanced</ion-label>
      </ion-range>
    </ion-item>
     <ion-card>
        <img src="http://dailypowerwalk.com/wp-content/uploads/2017/06/Excercise.jpg" />
        <ion-card-header>
          <ion-card-title>500 Calories Burn</ion-card-title>
          <ion-card-subtitle>
            <div style="display:flex">
            <div style="flex:1">Intermediate | </div>
            <div style="flex:1">500 calories | </div>
            <div style="flex:1">+ points </div>
            </div>
          </ion-card-subtitle>
        </ion-card-header>
      </ion-card>
       <ion-card>
        <img src="http://dailypowerwalk.com/wp-content/uploads/2017/06/Excercise.jpg" />
        <ion-card-header>
          <ion-card-title>500 Calories Burn</ion-card-title>
          <ion-card-subtitle>
            <div style="display:flex">
            <div style="flex:1"> Intermediate | </div>
            <div style="flex:1"> 500 calories | </div>
            <div style="flex:1"> + points </div>
            </div>
          </ion-card-subtitle>
        </ion-card-header>
      </ion-card>
       <ion-card>
        <img src="http://dailypowerwalk.com/wp-content/uploads/2017/06/Excercise.jpg" />
        <ion-card-header>
          <ion-card-title>500 Calories Burn</ion-card-title>
          <ion-card-subtitle>
            <div style="display:flex">
            <div style="flex:1"> Intermediate | </div>
            <div style="flex:1"> 500 calories | </div>
            <div style="flex:1"> + points </div>
            </div>
          </ion-card-subtitle>
        </ion-card-header>
      </ion-card>
       </ion-list>
</ion-content>
<template slot="bottom">
      <ion-tab-bar>
        <ion-tab-button tab="schedule">
          <ion-icon name="calendar"></ion-icon>
          <ion-label>Schedule</ion-label>
          <ion-badge>6</ion-badge>
        </ion-tab-button>

        <!-- Provide a custom route to navigate to -->
        <ion-tab-button tab="speakers" :to="{ name: 'app.speakers' }">
          <ion-icon name="person-circle"></ion-icon>
          <ion-label>Speakers</ion-label>
        </ion-tab-button>

        <!-- Provide extra data to route -->
        <ion-tab-button tab="map" :to="{ name: 'app.map', params: { mode: 'dark' } }">
          <ion-icon name="map"></ion-icon>
          <ion-label>Map</ion-label>
        </ion-tab-button>

        <!-- Provide custom click handler -->
        <ion-tab-button tab="about" @click="goToAboutTab">
          <ion-icon name="information-circle"></ion-icon>
          <ion-label>About</ion-label>
        </ion-tab-button>
      </ion-tab-bar>
    </template>
</ion-app>
</template>
<script>
export default {
  mounted () {
  },
  name: 'Home'
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>

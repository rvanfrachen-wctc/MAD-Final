<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Home</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Home</ion-title>
        </ion-toolbar>
      </ion-header>
    
      <div id="container">
        <p>Welcome to the photo gallery!</p>
        <br>
        <ion-list :inset="true">
          <ion-item>
            <ion-label>On the second tab you can take pictures and save them within the app.</ion-label>
          </ion-item>
          <ion-item>
            <ion-label>They are saved to your device so when you come back they will all be there.</ion-label>
          </ion-item>
          <ion-item>
            <ion-label>You can also delete them if you no longer would like them to be saved.</ion-label>
          </ion-item>
          <ion-item>
            <ion-label>This is great for saving select photos that you later want to share with family members or friends, you know right where to go.</ion-label>
          </ion-item>
        </ion-list>
      </div>

    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent, IonItem, IonLabel, IonList } from '@ionic/vue';

export default defineComponent({
  name: 'Tab1Page',
  components: { IonHeader, IonToolbar, IonTitle, IonContent, IonPage, IonItem, IonLabel, IonList }
});
</script>

<style scoped>
#container {
  text-align: center;
  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 22px;
  color: #8c8c8c;
  margin: 0;
}

#container a {
  text-decoration: none;
}
</style>

<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <Menu />
        <ion-title>Tab 1</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Tab 1</ion-title>
        </ion-toolbar>
      </ion-header>
    
      <ExploreContainer name="Tab 1 page" />
      <ion-list>
        <ion-item>
          <ion-label>Input</ion-label>
          <ion-input></ion-input>
        </ion-item>
        <ion-item>
          <ion-label>Toggle</ion-label>
          <ion-toggle slot="end"></ion-toggle>
        </ion-item>
        <ion-item>
          <ion-label>Radio</ion-label>
          <ion-radio slot="end"></ion-radio>
        </ion-item>
        <ion-item>
          <ion-label>Radio</ion-label>
          <ion-radio slot="end"></ion-radio>
        </ion-item>
        <ion-item>
          <ion-label>Checkbox</ion-label>
          <ion-checkbox slot="start"></ion-checkbox>
        </ion-item>
      </ion-list>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent, IonCheckbox, 
  IonInput, 
  IonItem, 
  IonList, 
  IonLabel, 
  IonRadio, 
  IonToggle  } from '@ionic/vue';
import ExploreContainer from '@/components/ExploreContainer.vue';
import Menu from '@/components/Menu.vue';

export default  {
  name: 'Tab1',
  components: { ExploreContainer, Menu, IonHeader, IonToolbar, IonTitle, IonContent, IonPage, IonCheckbox, 
    IonInput, 
    IonItem,
    IonList, 
    IonLabel, 
    IonRadio, 
    IonToggle  }
}
</script>
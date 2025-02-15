```html
<template>
  <ion-content>
    <ion-accordion-group>
      <ion-accordion value="first">
        <ion-item slot="header" color="light">
          <ion-label>First Accordion</ion-label>
        </ion-item>
        <div class="ion-padding" slot="content">
          First Content
        </div>
      </ion-accordion>
      <ion-accordion value="second" :disabled="true">
        <ion-item slot="header" color="light">
          <ion-label>Second Accordion</ion-label>
        </ion-item>
        <div class="ion-padding" slot="content">
          Second Content
        </div>
      </ion-accordion>
      <ion-accordion value="third">
        <ion-item slot="header" color="light">
          <ion-label>Third Accordion</ion-label>
        </ion-item>
        <div class="ion-padding" slot="content">
          Third Content
        </div>
      </ion-accordion>
    </ion-accordion-group>
  </ion-content>
</template>

<script lang="ts">
  import {
    IonAccordion, 
    IonAccordionGroup,
    IonContent,
    IonItem, 
    IonLabel,
    AccordionGroupCustomEvent
  } from '@ionic/vue';
  import { defineComponent, ref } from 'vue';
  export default defineComponent({
    components: {
      IonAccordion, 
      IonAccordionGroup,
      IonContent,
      IonItem, 
      IonLabel
    }
  });
</script>
```

---
title: "ion-note"
hide_table_of_contents: true
demoUrl: "/docs/demos/api/note/index.html"
demoSourceUrl: "https://github.com/ionic-team/ionic-docs/tree/main/static/demos/api/note/index.html"
---
import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';
import TOCInline from '@theme/TOCInline';

import Props from '@site/static/auto-generated/note/props.md';
import Events from '@site/static/auto-generated/note/events.md';
import Methods from '@site/static/auto-generated/note/methods.md';
import Parts from '@site/static/auto-generated/note/parts.md';
import CustomProps from '@site/static/auto-generated/note/custom-props.md';
import Slots from '@site/static/auto-generated/note/slots.md';

<head>
  <title>ion-note: Note Text Elements for iOS and Android Ionic Apps</title>
  <meta name="description" content="ion-notes are text elements generally used as subtitles that provide more information. Learn how notes can be used and styled on iOS and Android Ionic apps." />
</head>

import EncapsulationPill from '@components/page/api/EncapsulationPill';

<EncapsulationPill type="shadow" />

<h2 className="table-of-contents__title">Contents</h2>

<TOCInline
  toc={toc}
  maxHeadingLevel={2}
/>



Notes are text elements generally used as subtitles that provide more information. Notes are styled to appear grey by default. Notes can be used in an item as metadata text.




## Usage

<Tabs groupId="framework" defaultValue="angular" values={[{ value: 'angular', label: 'Angular' }, { value: 'javascript', label: 'Javascript' }, { value: 'react', label: 'React' }, { value: 'stencil', label: 'Stencil' }, { value: 'vue', label: 'Vue' }]}>

<TabItem value="angular">

```html
<!-- Default Note -->
<ion-note>Default Note</ion-note>

<!-- Note Colors -->
<ion-note color="primary">Primary Note</ion-note>
<ion-note color="secondary">Secondary Note</ion-note>
<ion-note color="danger">Danger Note</ion-note>
<ion-note color="light">Light Note</ion-note>
<ion-note color="dark">Dark Note</ion-note>

<!-- Notes in a List -->
<ion-list>
  <ion-item>
    <ion-label>Note (End)</ion-label>
    <ion-note slot="end">On</ion-note>
  </ion-item>

  <ion-item>
    <ion-note slot="start">Off</ion-note>
    <ion-label>Note (Start)</ion-label>
  </ion-item>
</ion-list>
```


</TabItem>


<TabItem value="javascript">

```html
<!-- Default Note -->
<ion-note>Default Note</ion-note>

<!-- Note Colors -->
<ion-note color="primary">Primary Note</ion-note>
<ion-note color="secondary">Secondary Note</ion-note>
<ion-note color="danger">Danger Note</ion-note>
<ion-note color="light">Light Note</ion-note>
<ion-note color="dark">Dark Note</ion-note>

<!-- Notes in a List -->
<ion-list>
  <ion-item>
    <ion-label>Note (End)</ion-label>
    <ion-note slot="end">On</ion-note>
  </ion-item>

  <ion-item>
    <ion-note slot="start">Off</ion-note>
    <ion-label>Note (Start)</ion-label>
  </ion-item>
</ion-list>
```


</TabItem>


<TabItem value="react">

```tsx
import React from 'react';
import { IonNote, IonList, IonItem, IonLabel, IonContent } from '@ionic/react';

export const NoteExample: React.FC = () => (
  <IonContent>
    {/*-- Default Note --*/}
    <IonNote>Default Note</IonNote><br />

    {/*-- Note Colors --*/}
    <IonNote color="primary">Primary Note</IonNote><br />
    <IonNote color="secondary">Secondary Note</IonNote><br />
    <IonNote color="danger">Danger Note</IonNote><br />
    <IonNote color="light">Light Note</IonNote><br />
    <IonNote color="dark">Dark Note</IonNote><br />

    {/*-- Notes in a List --*/}
    <IonList>
      <IonItem>
        <IonLabel>Note (End)</IonLabel>
        <IonNote slot="end">On</IonNote>
      </IonItem>

      <IonItem>
        <IonNote slot="start">Off</IonNote>
        <IonLabel>Note (Start)</IonLabel>
      </IonItem>
    </IonList>
  </IonContent>
);
```

</TabItem>


<TabItem value="stencil">

```tsx
import { Component, h } from '@stencil/core';

@Component({
  tag: 'note-example',
  styleUrl: 'note-example.css'
})
export class NoteExample {
  render() {
    return [
      // Default Note
      <ion-note>Default Note</ion-note>,

      // Note Colors
      <ion-note color="primary">Primary Note</ion-note>,
      <ion-note color="secondary">Secondary Note</ion-note>,
      <ion-note color="danger">Danger Note</ion-note>,
      <ion-note color="light">Light Note</ion-note>,
      <ion-note color="dark">Dark Note</ion-note>,

      // Notes in a List
      <ion-list>
        <ion-item>
          <ion-label>Note (End)</ion-label>
          <ion-note slot="end">On</ion-note>
        </ion-item>

        <ion-item>
          <ion-note slot="start">Off</ion-note>
          <ion-label>Note (Start)</ion-label>
        </ion-item>
      </ion-list>
    ];
  }
}
```


</TabItem>


<TabItem value="vue">

```html
<template>
  <!-- Default Note -->
  <ion-note>Default Note</ion-note>

  <!-- Note Colors -->
  <ion-note color="primary">Primary Note</ion-note>
  <ion-note color="secondary">Secondary Note</ion-note>
  <ion-note color="danger">Danger Note</ion-note>
  <ion-note color="light">Light Note</ion-note>
  <ion-note color="dark">Dark Note</ion-note>

  <!-- Notes in a List -->
  <ion-list>
    <ion-item>
      <ion-label>Note (End)</ion-label>
      <ion-note slot="end">On</ion-note>
    </ion-item>

    <ion-item>
      <ion-note slot="start">Off</ion-note>
      <ion-label>Note (Start)</ion-label>
    </ion-item>
  </ion-list>
</template>

<script>
import { IonItem, IonLabel, IonList, IonNote } from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  components: { IonItem, IonLabel, IonList, IonNote }
});
</script>
```


</TabItem>

</Tabs>

## Properties
<Props />

## Events
<Events />

## Methods
<Methods />

## CSS Shadow Parts
<Parts />

## CSS Custom Properties
<CustomProps />

## Slots
<Slots />
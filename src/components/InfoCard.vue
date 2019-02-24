<template>
    <q-card>
    <q-item>
    <q-item-side avatar="/statics/icons/icon-384x384.png"/>
    <q-item-main>
        <q-card-title>Kira
          <p slot="subtitle">It's How You Know What's In Your Contacts</p>
          <q-checkbox slot="right" v-model="checked"/>
        </q-card-title>
    </q-item-main>
    </q-item>
    <q-card-separator/>
    <q-card-main>
    <p>Kira is a powerful machine learning software that identifies, extacts, and analyzes text in your contracts and other documents</p>
    </q-card-main>
    </q-card>
</template>
<script>
export default {
  name: 'infoCard',
  data () {
    return {
      checked: false
    }
  }
}
</script>
<style>
/* This is where your CSS goes */
</style>

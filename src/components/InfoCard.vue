<template>
    <div class="container">
    <div v-for="(item, index) of items" :key="index">
    <q-card>
    <q-item>
    <q-item-side :avatar="item.avatar"/>
    <q-item-main>
        <q-card-title>{{ item.title }}
          <p slot="subtitle">{{ item.subtitle }}</p>
          <q-checkbox slot="right" v-model="checked"/>
        </q-card-title>
    </q-item-main>
    </q-item>
    <q-card-separator/>
    <q-card-main>
    <p>{{ item.description }}</p>
    </q-card-main>
    </q-card>
    </div>
    </div>
</template>
<script>
export default {
  name: 'InfoCard',
  data () {
    return {
      checked: false,
      items: [{ title: 'Kira', subtitle: `It's How You Know What's In Your Contracts`, avatar: `kira.jpg`, description: `Kira is a powerful machine learning software that identifies, extracts and analyzes text in your contracts and other documents` }, { title: 'Doxly', subtitle: `Secure Portal for End to End Transactions`, avatar: `doxly.jpg`, description: `Manage the entire legal transaction process from dilligence to closing` }, { title: 'Clause', subtitle: `Connected Contracting`, avatar: `clause.jpg`, description: `Clause builds the technology infrastructure for connected contracts to increase the vlaue and improve the management of your business agreements` }]
    }
  }
}
</script>
<style>

.container {
  padding: 10px;
}
</style>

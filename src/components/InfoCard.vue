<template>
    <div class="row">
    <div class="col-4 q-pa-sm" v-for="(item, index) of items" :key="index">
    <div>
    <q-card>
    <q-item class="row">
    <q-item-side :image="item.avatar"/>
    <q-item-main class="q-ma-xs">
        <q-card-title>{{ item.title }}
          <p slot="subtitle">{{ item.subtitle }}</p>
          <q-checkbox slot="right" v-model="item.checked" color="secondary"/>
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
    </div>
</template>
<script>
export default {
  name: 'InfoCard',
  data () {
    return {
      items: [{ title: 'Kira', subtitle: `It's How You Know What's In Your Contracts`, avatar: `../statics/logos/kira.png`, description: `Kira is a powerful machine learning software that identifies, extracts and analyzes text in your contracts and other documents`, checked: false }, { title: 'Doxly', subtitle: `Secure Portal for End to End Transactions`, avatar: `../statics/logos/doxly.png`, description: `Manage the entire legal transaction process from dilligence to closing`, checked: false }, { title: 'Clause', subtitle: `Connected Contracting`, avatar: `../statics/logos/clause.png`, description: `Clause builds the technology infrastructure for connected contracts to increase the vlaue and improve the management of your business agreements`, checked: false }]
    }
  }// default data stored as an array here, breaking up this long line of code causes lint issues.
}
</script>

<template>
  <div id="app">
    <div class="demo">
      <span class="label">default:</span>
      <date-picker v-model="value1" lang="en"></date-picker>
    </div>
    <div class="demo">
      <span class="label">range:</span>
      <date-picker v-model="value2" range lang="zh"></date-picker>
    </div>
  </div>
</template>

<script>
import DatePicker from '../datepicker/index.vue'

export default {
  name: 'app',
  components: { DatePicker },
  data () {
    return {
      value1: '2017-5-9',
      disabledDays: ['2017-8-13'],
      notAfter: '2017-9-16',
      value2: ''
    }
  }
}
</script>

<style>
.demo {
  float:left;
  margin:250px;
}
.label{
  margin-right: 1em;
}
</style>

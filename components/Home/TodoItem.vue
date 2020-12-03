<template>
  <div class="todo-item">
    <v-checkbox v-model="value" hide-details :class="{ 'is-checked' : value }">
      <template #label>
        <span>Morning Walk</span>
        <v-spacer/>
        <span class="time">7am</span>
      </template>
    </v-checkbox>
  </div>
</template>

<script>
export default {
  data () {
    return {
      value: true
    }
  }
}
</script>

<style lang="scss">
.todo-item {
  margin-bottom: 30px;
  > .v-input--selection-controls .v-input__slot > .v-label, .v-input--selection-controls .v-radio > .v-label{
    color: #65656A;
    line-height: 30px;
    border-bottom: 1px solid #D0D0D1;
  }

  .time {
    font-size: 14px;
  }

  .is-checked.v-input--selection-controls .v-input__slot > .v-label, .v-input--selection-controls .v-radio > .v-label {
    color: #D0D0D1;
    border-bottom: none;
    text-decoration: line-through;
  }
}
</style>

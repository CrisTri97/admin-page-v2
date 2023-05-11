<template>
  <div>
    <div class="center content-inputs form-container">
      <vs-input class="input-item" v-model="value1" type="text" label="Text" />
      <vs-input
        class="input-item"
        v-model="value2"
        type="password"
        label="Password"
      />
      <vs-input
        class="input-item"
        v-model="value3"
        type="search"
        label="Search"
      />
      <vs-input
        class="input-item"
        v-model="value4"
        type="number"
        label="Number"
      />
      <vs-input class="input-item" v-model="value5" type="url" label="Url" />
      <vs-input class="input-item" v-model="value6" type="time" label="time" />
      <vs-input class="input-item" v-model="value7" type="date" label="Date" />
      <vs-select
        label-placeholder="Label-placeholder"
        v-model="value8"
      >
        <vs-option label="Vuesax" value="1">
          Vuesax
        </vs-option>
        <vs-option label="Vue" value="2">
          Vue
        </vs-option>
        <vs-option label="Javascript" value="3">
          Javascript
        </vs-option>
        <vs-option label="Sass" value="4">
          Sass
        </vs-option>
        <vs-option label="Typescript" value="5">
          Typescript
        </vs-option>
        <vs-option label="Webpack" value="6">
          Webpack
        </vs-option>
        <vs-option label="Nodejs" value="7">
          Nodejs
        </vs-option>
      </vs-select>
    </div>
    <ListUpload />
  </div>
</template>
<script>
export default {
  data: () => ({
    value1: '',
    value2: '',
    value3: '',
    value4: '',
    value5: '',
    value6: '',
    value7: '',
    value8: '',
  }),
}
</script>
<style lang="scss">
.form-container {
  display: flex;
  flex-wrap: wrap;
  gap: 30px;
  padding: 30px 5px;
  border: 1.5px solid rgb(228, 225, 225);
  .input-item {
  }
}
</style>

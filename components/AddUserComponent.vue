<template>
  <div class="add-user-container">
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
      <vs-select v-model="value8" label-placeholder="Label-placeholder">
        <vs-option label="Vuesax" value="1"> Vuesax </vs-option>
        <vs-option label="Vue" value="2"> Vue </vs-option>
        <vs-option label="Javascript" value="3"> Javascript </vs-option>
        <vs-option label="Sass" value="4"> Sass </vs-option>
        <vs-option label="Typescript" value="5"> Typescript </vs-option>
        <vs-option label="Webpack" value="6"> Webpack </vs-option>
        <vs-option label="Nodejs" value="7"> Nodejs </vs-option>
      </vs-select>
    </div>
    <div class="form-container">
      <ListingDetail />
      <SelectComponent :values="values" placeholder="I did" />
      <SelectComponent :values="values" placeholder="I finished products" />
      <SelectComponent :values="values" placeholder="2022 - 2023" />
      <div class="centerx input-search">
        <vs-input
          v-model="value2"
          color="#7d33ff"
          border
          type="password"
          placeholder="Search"
        >
          <template #icon>
            <i class="bx bx-search"></i>
          </template>
        </vs-input>
      </div>

      <VsChip :value="valueChip" />
      <SelectComponent
        class="select-color"
        :values="values"
        placeholder="Pinks"
      />
      <SelectComponent
        class="select-color"
        :values="values"
        placeholder="Choose second color"
      />
      <TextAreaCheckBox />
      <SelectComponent
        class="select-color"
        :values="values"
        placeholder="Boho & hippie"
      />
      <SelectComponent
        class="select-color"
        :values="values"
        placeholder="Baches color party"
      />
      <SelectComponent
        class="select-color"
        :values="values"
        placeholder="Thanksgiving"
      />
      <RadioRenewalOption/>
    </div>
    <!-- <ListUpload /> -->
  </div>
</template>
<script>
import RadioRenewalOption from './RadioRenewalOption.vue';
import SelectComponent from './SelectComponent.vue'
import TextAreaCheckBox from './TextAreaCheckBox.vue'
import VsChip from './VsChip.vue'

export default {
  components: { SelectComponent, VsChip, TextAreaCheckBox, RadioRenewalOption },
  data: () => ({
    value1: '',
    value2: '',
    value3: '',
    value4: '',
    value5: '',
    value6: '',
    value7: '',
    value8: '',
    values: [
      {
        id: 1,
        label: 'a',
        value: 'a',
      },
      {
        id: 2,
        label: 'b',
        value: 'b',
      },
      {
        id: 3,
        label: 'c',
        value: 'c',
      },
    ],
    valueChip: ['Bags & Purses', 'Handbags', 'Cross body bags'],
  }),
}
</script>
<style lang="scss">
.add-user-container {
  .form-container {
    display: flex;
    flex-wrap: wrap;
    gap: 30px;
    padding: 30px 5px;
    border: 1.5px solid rgb(228, 225, 225);
    margin-bottom: 10px;
    .select-color {
      width: 100%;
    }
    .input-item {
    }
  }
  .input-search {
    width: 100%;
    input {
      width: 100%;
    }
  }
}
</style>

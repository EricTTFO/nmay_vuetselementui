<template>
  <div>
    <el-time-picker
      v-model="value2"
      :picker-options="{
      selectableRange: '18:30:00 - 20:30:00'
    }"
      placeholder="任意时间点"
    ></el-time-picker>
    <el-time-picker
      arrow-control
      v-model="value3"
      :picker-options="{
      selectableRange: '18:30:00 - 20:30:00'
    }"
      placeholder="任意时间点"
    ></el-time-picker>
  </div>
</template>

<script lang="ts">
import { Component, Vue, Model, Prop } from "vue-property-decorator";

@Component({
  components: {}
})
export default class Navbar extends Vue {
  @Prop() private msg!: string;
  public value2: any = new Date(2016, 9, 10, 18, 40);
  public value3: any = new Date(2016, 9, 10, 18, 40);
}
</script>

<style>
</style>

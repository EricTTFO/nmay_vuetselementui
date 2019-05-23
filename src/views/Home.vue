<template>
  <div class="home">
    我是home
    <layout/>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';
import layout from './layout/layout.vue';


@Component({
  components: {
    layout
  }
})
export default class Home extends Vue {
  @Prop() private msg!: string;
}
</script>

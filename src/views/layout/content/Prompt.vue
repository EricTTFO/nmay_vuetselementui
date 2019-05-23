<template>
<div>
    asdprompt
</div>
</template>
<script lang="ts">
import { Component, Vue, Model, Prop } from "vue-property-decorator";

@Component({
  components: {}
})
export default class Promat extends Vue {
  @Prop() private msg!: string;
}
</script>

<style>
</style>

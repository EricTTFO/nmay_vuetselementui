<template>
  <div>
    <div class="t-container">
      <div class="t-navbar-con">
        <!-- 左侧导航 -->
        <Navbar/>
      </div>
      <!-- 主要内容 -->
      <div class="t-po-r">
        <Main/>
        <div class="MainBo"></div>
        <div class="t-prompt-content">
          <Prompt/>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue, Model, Prop } from "vue-property-decorator";
import Main from "./content/Main.vue";
import Navbar from "./content/Navbar.vue";
import Prompt from "./content/Prompt.vue";

@Component({
  components: {
    Main,
    Navbar,
    Prompt
  }
})
export default class layout extends Vue {
  @Prop() private msg!: string;
}
</script>


<style>
</style>

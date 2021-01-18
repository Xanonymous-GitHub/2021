<template>
  <div class="cfp">
    <!-- <h1>cfp</h1> -->
    <Info />
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

// import Agenda from "../components/CFP/Agenda.vue";
import Info from "./Info.vue";

@Component({
  components: {
    Info,
  },
})
export default class CFP extends Vue {
  @Prop() private msg!: string;
}
</script>

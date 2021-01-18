<template>
  <div class="cfp">
    <!-- <h1>cfp</h1> -->
    <Agenda />
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

import Agenda from "../components/CFP/Agenda.vue";

@Component({
  components: {
    Agenda,
  },
})
export default class CFP extends Vue {
  @Prop() private msg!: string;
}
</script>

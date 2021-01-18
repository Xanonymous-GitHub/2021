<template>
  <div class="info">
    <SubInformation />
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
// components
import SubInformation from "../components/CFP/SubInformation.vue";

@Component({
  components: {
    SubInformation,
  },
})
export default class Info extends Vue {
  @Prop() private msg!: string;
}
</script>

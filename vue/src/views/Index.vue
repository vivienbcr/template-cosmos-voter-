<template>
  <div>
    <div class="sp-container">
      <sp-sign-in />
      <sp-bank-balances />
      <sp-token-send />
      <!-- this line is used by starport scaffolding # 4 -->
		<sp-type-form type="poll" :fields="['title', 'options', ]" module="voter" />
      <app-text type="h1">voter</app-text>
      <wallet />
      <poll-form />
      <poll-list />
    </div>
  </div>
</template>

<script>
import * as sp from "@tendermint/vue";


export default {
  components: { ...sp },
};
</script>

<template lang="pug">
  div
    h2 Examples
    client-only(placeholder="loading...")
      BaseExample
      <BaseWithSaveView />
      template(v-if="['portal', 'brightspeed', 'portalrebrand24'].includes(selectedTheme)")
      <BaseWithSaveViewAndBulkActionsPortalBrightSpeed />
</template>

<script lang="ts">
import { Vue } from 'vue-facing-decorator';
import Base from './_base.vue';
import BaseWithSaveView from './_base-with-save-view.vue';
import BaseWithSaveViewAndBulkActionsPortalBrightSpeed from './_portal/_base-with-save-view-bulk-actions.vue';

@NuxtComponent({
  components: {
    BaseExample: Base,
    BaseWithSaveView,
    BaseWithSaveViewAndBulkActionsPortalBrightSpeed,
  },
})
export default class Examples extends Vue {
  selectedTheme = useSelectedTheme();
}
</script>

<template lang="pug">
  div
    h2 Examples
    p.-text
      | A dropdown must be associated with an activator, commonly a button, which, at the time of being clicked, expands
      | the dropdown. Activator and dropdown should be contained in a div with a <code>chi-dropdown</code> class, or otherwise, the
      | activator must reference the dropdown with a <code>data-target</code> attribute.
      | Use the <code>chi-dropdown__trigger</code> class on your activator button to make the chevron appear.

    BaseExample
    <AdditionalStyles />
    <HelperMessage />
    <DataTarget />
    <Hover />
    <Animated />
    <Positioning />

    h3 Menu
    <States />
    <Description />
    <Divider />
    <Icons />
    <SearchBox />
    <VisibleItems />
    <RetainSelection />

    ClientOnly
      SelectMode
    <IconTrigger />

    h3 Checkboxes
    <CheckboxesBase />
    <CheckboxesIcons />

    <RadioButtons />
    <RangeInput />
    <ToggleSwitch />
    <PlainText />

    h3 Helpers
    <TruncateLongMenuItems />
    <FlexibleHeight />
</template>

<script lang="ts">
import { Vue } from 'vue-facing-decorator';
import Base from './_base.vue';
import AdditionalStyles from './_additional_styles.vue';
import DataTarget from './_data_target.vue';
import Hover from './_hover.vue';
import Animated from './_animate.vue';
import Positioning from './_positioning.vue';
import States from './_states.vue';
import Description from './_description.vue';
import Divider from './_divider.vue';
import Icons from './_icons.vue';
import SearchBox from './_search_box.vue';
import CheckboxesBase from './_checkboxes_base.vue';
import CheckboxesIcons from './_checkboxes_icons.vue';
import RadioButtons from './_radio_buttons.vue';
import RangeInput from './_range_input.vue';
import ToggleSwitch from './_toggle_switch.vue';
import PlainText from './_plain_text.vue';
import TruncateLongMenuItems from './_truncate_long_menu_items.vue';
import FlexibleHeight from './_flexible_height.vue';
import VisibleItems from './_visible_items.vue';
import RetainSelection from './_retain_selection.vue';
import IconTrigger from './_icon_trigger.vue';
import SelectMode from './_select_mode.vue';
import HelperMessage from './_helper_message.vue';

@NuxtComponent({
  components: {
    Animated,
    BaseExample: Base,
    AdditionalStyles,
    CheckboxesBase,
    CheckboxesIcons,
    DataTarget,
    Description,
    Divider,
    FlexibleHeight,
    Hover,
    Icons,
    PlainText,
    Positioning,
    RadioButtons,
    RangeInput,
    SearchBox,
    States,
    ToggleSwitch,
    TruncateLongMenuItems,
    VisibleItems,
    RetainSelection,
    IconTrigger,
    SelectMode,
    HelperMessage,
  },
})
export default class Examples extends Vue { }
</script>

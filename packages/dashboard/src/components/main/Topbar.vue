<template>
  <q-btn dense flat round icon="menu" @click="$emit('toggle')" />
  <q-space />
  <bucket-picker/>
</template>

<script>
import BucketPicker from "components/main/BucketPicker.vue";
import { defineComponent } from "vue";

export default defineComponent({
	name: "TopBar",
	emits: ["toggle"],
	components: { BucketPicker },
});
</script>

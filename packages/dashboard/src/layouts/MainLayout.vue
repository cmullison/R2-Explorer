<template>
  <q-layout view="hHh LpR lFr">

    <q-header reveal class="bg-[#423fad] text-white">
      <q-toolbar>

        <top-bar @toggle="toggleLeftDrawer"/>

      </q-toolbar>
    </q-header>

    <q-drawer :width="100" show-if-above v-model="leftDrawerOpen" side="left" bordered>
      <left-sidebar/>
    </q-drawer>

<!--    <q-drawer show-if-above v-model="rightDrawerOpen" side="right" bordered>-->
<!--      <right-sidebar @updateDrawer="updateRightDrawer" />-->
<!--    </q-drawer>-->

    <q-page-container>
      <router-view />
    </q-page-container>

  </q-layout>
</template>

<script>
import LeftSidebar from "components/main/LeftSidebar.vue";
import RightSidebar from "components/main/RightSidebar.vue";
import TopBar from "components/main/Topbar.vue";
import { ref } from "vue";

export default {
	name: "MainLayout",
	components: { TopBar, RightSidebar, LeftSidebar },
	setup() {
		const leftDrawerOpen = ref(false);
		const rightDrawerOpen = ref(false);

		return {
			leftDrawerOpen,
			toggleLeftDrawer() {
				leftDrawerOpen.value = !leftDrawerOpen.value;
			},

			rightDrawerOpen,
			updateRightDrawer(state) {
				rightDrawerOpen.value = state;
			},
		};
	},
	mounted() {
		this.updateRightDrawer(false);
	},
};
</script>

<template>
	<v-container
		class="v--flex v--flex-justify-center v--flex-column v--full-height v--text-inverse home"
	>
		<h1 class="icon">🔐</h1>
		<h1><b v-t="'home.welcome'" /></h1>
		<p v-t="'home.please-auth'" />
	</v-container>
</template>
<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import VContainer from "@/components/ui/layout/VContainer.vue";
@Component({
	components: { VContainer },
})
export default class Home extends Vue {}
</script>
<style lang="scss" scoped>
.home {
	h1 {
		font-size: 4em;

		&.icon {
			font-size: 6em;
		}
	}

	p {
		font-size: 18px;
		margin-top: 8px;
	}
}
</style>

<template>
	<NuxtLink :class="styled ? '' : 'text-main hover:no-underline'" :to="localePath(to)"><slot /></NuxtLink>
</template>

<script>
export default {
	props: {
		to: {
			type: String,
			required: true,
		},
		styled: {
			type: Boolean,
			default: true,
		},
	},
}
</script>

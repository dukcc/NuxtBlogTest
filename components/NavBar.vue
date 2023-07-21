<template>
	<nav
		class="flex gap-[64px] w-full h-fit align-middle place-items-center place-content-center"
	>
		<nuxt-link
			to="/"
			:class="[
				{
					'text-[20px] font-medium cursor-pointer hover:opacity-75 duration-200 selected':
						home,
				},
				{
					'text-[20px] font-medium cursor-pointer hover:opacity-75 duration-200':
						posts,
				},
			]"
		>
			Home
		</nuxt-link>
		<nuxt-link
			to="/postslist"
			:class="[
				{
					'text-[20px] font-medium cursor-pointer hover:opacity-75 duration-200':
						home,
				},
				{
					'text-[20px] font-medium cursor-pointer hover:opacity-75 duration-200 selected':
						posts,
				},
			]"
		>
			Posts
		</nuxt-link>
	</nav>
</template>

<script>
export default {
	props: {
		selected: {
			type: String,
			default: "home",
		},
	},

	computed: {
		home() {
			return this.selected === "home";
		},
		posts() {
			return this.selected === "posts";
		},
	},
};
</script>

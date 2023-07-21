<template>
	<div
		class="bg-black text-white h-screen w-screen flex flex-col p-[64px] gap-[64px]"
	>
		<NavBar selected="posts" />
		<div
			class="bg-[url(/head.jpg)] bg-cover text-black rounded-xl p-[128px] w-full flex flex-col gap-[32px]"
		>
			<h1 class="text-4xl font-bold w-fit">Posts List</h1>
			<h4 class="text-2xl w-fit">h</h4>
		</div>
		<div class="grid grid-rows-auto grid-cols-3 gap-[64px] h-96 bg-black">
			<ContentList path="/posts" v-slot="{ list }">
				<NuxtLink class="bg-[#111111] p-[32px] rounded-xl flex flex-col gap-[16px]" v-for="post in list" :key="post._path" :to="post._path" >
					<h2 class="text-3xl font-bold">{{ post.title }}</h2>
					<p>{{ post.description }}</p>
				</NuxtLink>
			</ContentList>
		</div>
	</div>
</template>

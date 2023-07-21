<template>
	<div
		class="bg-black text-white h-screen w-screen flex flex-col p-[64px] gap-[64px]"
	>
		<NavBar />
		<div
			class="bg-[url(/head.jpg)] bg-cover text-black rounded-xl p-[128px] w-full flex flex-col gap-[32px]"
		>
			<h1 class="text-4xl font-bold w-fit">Nuxt Blog Text</h1>
			<h4 class="text-2xl w-fit">h</h4>
		</div>
		<div class="flex place-items-center gap-[64px] h-96 bg-black">
			<NuxtLink to="/postslist">
                <LargeButton text="View Posts" />
            </NuxtLink>
		</div>
	</div>
</template>

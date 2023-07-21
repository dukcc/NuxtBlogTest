<template>
	<main
		class="bg-black text-white flex flex-col align-middle p-[64px] h-screen w-screen"
	>
		<NavBar selected="posts" />
		<article
			class="prose lg:prose-xl prose-h1:text-white prose-h2:text-white prose-h3:text-white prose-h4:text-white prose-h6:text-white prose-p:text-[#e1e1e1] prose-a:text-[#4abeff] hover:prose-a:text-[#a4deff] prose-code:text-[#b3b3b3] prose-li:text-[#e1e1e1] prose-ul:text-[#e1e1e1] prose-blockquote:text-[#e1e1e1]"
		>
			<ContentDoc />
		</article>
	</main>
</template>
<!-- YOU CAN DELETE EVERYTHING IN THIS PAGE -->
	<script lang="ts">
		import { Avatar } from '@skeletonlabs/skeleton';
		import logo from "$lib/images/logo2.png";
	</script>
<div class="container h-full mx-auto flex justify-center items-center">
	<div class="space-y-10 text-center flex flex-col items-center">
		<Avatar src={logo} width="w-64" rounded="rounded-full" class="m-0 p-0" />
		<h2 class="h2">Hi! I'm YuneKomori👋</h2>

		<!-- ボタンのラップ要素で横並びにする -->
		<div class="flex justify-center space-x-2 w-full">
			<!-- 最新のブログを読むボタン -->
			<a
				class="btn variant-filled w-full text-center"
				href="https://skeleton.dev/"
				target="_blank"
				rel="noreferrer"
			>
				最新のブログを読む
			</a>

			<!-- About meボタン -->
			<a
				class="btn variant-filled w-full text-center"
				href="https://skeleton.dev/"
				target="_blank"
				rel="noreferrer"
			>
				About me
			</a>
		</div>

		<div class="space-y-2">
			<p>Try editing the following:</p>
			<p><code class="code">/src/routes/+layout.svelte</code></p>
			<p><code class="code">/src/routes/+page.svelte</code></p>
		</div>
	</div>
</div>


<style lang="postcss">
	figure {
		@apply flex relative flex-col;
	}
	figure svg,
	.img-bg {
		@apply w-64 h-64 md:w-80 md:h-80;
	}
	.img-bg {
		@apply absolute z-[-1] rounded-full blur-[50px] transition-all;
		animation: pulse 5s cubic-bezier(0, 0, 0, 0.5) infinite,
			glow 5s linear infinite;
	}

	@keyframes glow {
		0% {
			@apply bg-primary-400/50;
		}
		33% {
			@apply bg-secondary-400/50;
		}
		66% {
			@apply bg-tertiary-400/50;
		}
		100% {
			@apply bg-primary-400/50;
		}
	}
	@keyframes pulse {
		50% {
			transform: scale(1.5);
		}
	}
</style>

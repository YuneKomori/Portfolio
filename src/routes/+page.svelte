<script lang="ts">
	import { Avatar } from '@skeletonlabs/skeleton';
	import logo from "$lib/images/logo2.png";
  </script>
  
  <div class="container h-full mx-auto flex justify-center items-center">
	<!-- Flexboxを使って左右に分割 -->
	<div class="flex w-full flex-col md:flex-row justify-between items-center space-x-0 md:space-x-10">
	  <!-- 左側：画像 -->
	  <div class="flex-shrink-0 mb-4 md:mb-0">
		<Avatar src={logo} width="w-32 md:w-80" rounded="rounded-full"  />
	  </div>
  
	  <!-- 右側：テキストとボタン -->
	  <div class="flex-grow text-center md:text-right space-y-10">
		<!-- レスポンシブなテキストサイズ -->
		<h2 class="h2 text-2xl md:text-4xl lg:text-6xl font-bold">Hi! I'm YuneKomori👋</h2>
  
		<!-- ボタンをレスポンシブで横並びに配置 -->
		<div class="flex flex-col md:flex-row justify-center md:justify-end space-y-2 md:space-y-0 md:space-x-2 w-full">
		  <a
			class="btn variant-filled w-full md:w-auto text-center"
			href="https://skeleton.dev/"
			target="_blank"
			rel="noreferrer"
		  >
			最新のブログを読む
		  </a>
  
		  <a
			class="btn variant-filled w-full md:w-auto text-center"
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
		<div>
			<div class="space-y-2">
				<p>My skil</p>
				<p><code class="code">/src/routes/+layout.svelte</code></p>
				<p><code class="code">/src/routes/+page.svelte</code></p>
			  </div>
		</div>
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
	  animation: pulse 5s cubic-bezier(0, 0, 0, 0.5) infinite, glow 5s linear infinite;
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
  
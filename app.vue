<script
	setup
>
import Toaster from '@/components/ui-kit/toast/Toaster.vue';
</script>

<template>
	<div class="background">
		<NuxtRouteAnnouncer />
		<NuxtLayout>
			<NuxtPage />
		</NuxtLayout>
		<Toaster />
	</div>
</template>

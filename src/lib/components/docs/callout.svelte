<script lang="ts">
	import * as Alert from "$lib/components/ui/alert/index.js";
</script>

<Alert.Root {...$$restProps} class="mt-2">
	{#if $$slots.icon}
		<span class="mr-4 text-2xl">
			<slot name="icon" />
		</span>
	{/if}
	<Alert.Title>
		<slot name="title" />
	</Alert.Title>
	<Alert.Description>
		<slot />
	</Alert.Description>
</Alert.Root>

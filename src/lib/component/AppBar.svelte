<script lang="ts">
	import { totalOrderCount } from "$lib/store/order";

    Import {totalOrderCount} from '$lib/store/order';
	Import {totalOrderCount, toalOrderValue} from '$lib/store/order';
</script>

<div class="appbar">Kongkow Cafe ({$totalOrderCount})</div>


<style>
    appbar {
	display: flex;
		flex-direction: row;
		justify-content: center;
		padding: 16px;
		background-color: #f44336;
		color: white;
		font-size: 16px;
		font-weight: 500;
    }
</style>
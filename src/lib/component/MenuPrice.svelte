<script>
    export let label:String;
    export let price:Number;
</script>

<div><div class="menu-price-row">
    <span class="price-description">{label}</span>
    <span>{price}</span>
    <div>
        <span class="price-description">{label}</span>
    <span>{price}</span>
    </div>
</div>

</div>
<style>
    div.menu-tile {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding-bottom: 16px;
	}

	div.menu-photo img {
		aspect-ratio: 1;
		object-fit: cover;
		max-width: 100%;
	}

	div.menu-tile-name {
		font-weight: 500;
		font-size: 16px;
		padding: 8px 16px;
		align-self: stretch;
		text-align: center;
	}

	div.menu-tile-description {
		font-size: 12px;
		align-self: stretch;
		text-align: center;
		padding: 0px 16px;
		height: 60px;
		padding-bottom: 16px;
	}

	div.menu-price-row {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		align-items: center;
		padding: 0 16px;
	}

	span.price-description {
		font-size: 12px;
	}
</style>
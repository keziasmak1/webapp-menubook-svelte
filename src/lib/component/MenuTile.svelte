export let photoUrl: string;
export let prices: { id: string; label: string; price: number }[];
$: counter = $order[id] ?? 0;
$: counter = Object.keys($order)
	.filter((e) => e.startsWith(id))
	.reduce((prev, curr) => {
		return prev + $order[curr];
	}, 0);
</script>

<div class="menu-tile">
@@ -55,22 +59,4 @@
	height: 60px;
	padding-bottom: 16px;
}
button {
	padding: 8px 16px;
	border: none;
}
button.add {
	background-color: #f44336;
	color: white;
	margin-bottom: 8px;
	margin-top: 16px;
}
button.substract {
	border: 1px solid #f44336;
	color: #f44336;
	background-color: white;
}
</style>
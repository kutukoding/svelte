<script>
	let src = 'https://svelte.dev/tutorial/image.gif';
	let imgAlt = 'Rick Astley';
</script>

<h2>step-2: image</h2>
<!-- src={src} 	==>> ini tidak perlu ditulis sepanjang ini karena variablenya sudah sama dgn attributesnya-->
<img {src} alt="{imgAlt} dances.">
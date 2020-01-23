<script>
    let coba = 'nested'
    //  `   adalah seperti <pre> bisa digunakan jika element/isi butuh lebih dari 1 baris
    let string = `this <i>string</i> 
        <a href='google.com'>contains</a> some 
        <strong>HTML!!!</strong>`
</script>

<h2>step-1: nested components</h2>
<p>Hello {coba.toUpperCase()}!</p>
<p>{@html string}</p>
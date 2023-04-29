<script>
  export let data ;

  var products = data.Sheet1 ;
  
  import {page} from '$app/stores';

  var productid = $page.params.productid ;

  console.log(productid);

  var myProduct = products.filter(function (item) {return item.ProductID == productid});

  var product = myProduct[0];

  console.log(product);



</script>



<h1>Hello this is svelte - {product.Price} </h1>

<ul>
	{#each products as product}
	<div>
   <h1>{product.ProductName}</h1>
   <h2>{product.Price}</h2>
   <h3>{product.ProductID}</h3>
   <img src={product.Images} alt="">
</div>
	{/each}
</ul>



<style>
   
</style>
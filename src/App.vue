<script>
export default {
	data() {
	return {
		text: 'page',
		href: 'page.html',
    name: 'john',
		surn: 'smit',
    var1: 1,
		var2: 2,
    num: 5,
		num1: 1,
		num2: 2,
		num3: 3,
    
}
}}

</script>
<template>
 <div id="app">
		Hello World
    <a href="page.html">page</a>
    3
	</div>
  <p>{{ name }}</p>
	<p>{{ surn }}</p>
	<img :src="attr">

  	{{ var1 + var2 }}
    {{  num * num}}
  	{{ num1 + num2 + num3 }}
</template>ru 
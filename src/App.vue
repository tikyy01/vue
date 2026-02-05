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
		arr1: [1, 2, 3],
		arr2: ['x', 'y', 'z'],
		arr3: [1, 2, 3],
		obj: {a: 1, b: 2, c: 3},
		obj: {x: 1, y: 2, z: 3},
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

	{{ arr1[0] }}
	{{ arr1[1] }}
	{{ arr1[2] }}
	<p>{{ arr2[0] }}</p>
	<p>{{ arr2[1] }}</p>
	<p>{{ arr2[2] }}</p>
	<p>{{ arr3[0] + arr3[1] + arr3[2] }}</p>
	{{ obj.a }}
	{{ obj.b }}
	{{ obj.c }}
	{{ obj.x + obj.y + obj.z }}
</template>ru 
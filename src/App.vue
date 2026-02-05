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
		obj: {x: 1, y: 2, z: 3},
		text: 'Начальное значение'
	}
},
  methods: {
    showDate: function() {
      const now = new Date();
	  alert(new Date().toLocaleString());
    },
	showSum: function() {
      alert(this.num1 + this.num2);
	},
	 getDayName(dayNumber) {
      const days = [
        'Воскресенье',
        'Понедельник',
        'Вторник',
        'Среда',
        'Четверг',
        'Пятница',
        'Суббота'
      ];
      if (dayNumber < 0 || dayNumber > 6 || isNaN(dayNumber)) {
        return 'Неверный номер дня';
      }
      
      return days[dayNumber];
    },
    
    showTodayDay() {
      const today = new Date();
      const dayIndex = today.getDay();
      const dayName = this.getDayName(dayIndex);
      
      alert(`Сегодня: ${dayName}`);
    },
	showSquare: function(num) {
      alert(num * num);
    },
	change1: function() {
      this.text = 'Первое значение';
    },
    change2: function() {
      this.text = 'Второе значение';
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
	{{ showDate() }}
	<p><button @click="showDate">Показать дату (клик)</button></p>
	<button @mouseenter="showDate">Показать дату (наведение)</button>
	{{ showSum() }}
	<p><button @click="showTodayDay">Показать название сегодняшнего дня недели</button></p>
	<p><button @click="showSquare(2)">Квадрат числа 2</button></p>
    <p><button @click="showSquare(3)">Квадрат числа 3</button></p>
	<p>{{ text }}</p>
	<button @click="change1">Изменить текст</button>
	<button @click="change1">Первый текст</button>
    <button @click="change2">Второй текст</button>
</template>ru 


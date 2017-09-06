<template>
	<div id="datas">
		<ul>
			<li v-for="mydata in datas" v-on:click="mydata.show =! mydata.show">
				<h2>{{ mydata.name }}</h2>
				<h3 v-show="mydata.show">{{ mydata.speciality }}</h3>
			</li>
		</ul>
	</div>
</template>

<script>
export default {
  data () {
    return {
     	datas:[
     		{name:'AAA',speciality:'Vue Components',show:false},
     		{name:'BBB',speciality:'HTML Wizardry',show:false},
     		{name:'CCC',speciality:'Click Events',show:false},
     		{name:'DDD',speciality:'Coditionals',show:false},
     		{name:'EEE',speciality:'Webpack',show:false},
     		{name:'FFF',speciality:'Data Diggin',show:false}
		]
    }
  }
}
</script>

<style scoped>
	#datas{
		width: 100%;
		max-width: 1200px;
		margin: 40px auto;
		padding: 0 20px;
		box-sizing: border-box;
	}
	ul{
		display: flex;
		flex-wrap: wrap;
		list-style-type: none;
		padding: 0;
	}
	li{
		flex-grow: 1;
		flex-basis: 300px;
		text-align: center;
		padding: 30px;
		border: 1px solid #222;
		margin: 10px;
	}
</style>

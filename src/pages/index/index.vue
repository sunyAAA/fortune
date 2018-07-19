<template>
	<div class="container">
		<img src="../../../static/logo.jpeg" alt="">
		<h2>笔画测凶吉</h2>
		<input type="text" v-model="name">
		<button>点我测算</button>
		<div class="box">
			<p class="text">{{result}}</p>
		</div>
	</div>
</template>

<script>
import cnchr from '../../common/js/cnchr.js';
export default {
    data() {
        return {
            motto: "Hello World",
            userInfo: {},
            name: "",
			result:''
        };
	},
	mounted(){
		console.log(cnchr.stroke('骄傲骄'))
	}
};
</script>

<style lang="stylus" scoped>
baseColor =  #9d9087
lightColor = #d1c7b7
darkColor = #7c8577
textColor = #f15a22
.container {
	overflow: hidden;
}
h2
	margin 10px
	font-size 18px
	text-align center
	color baseColor
input 
	margin 0 auto
	width 80%
	border  1px solid lightColor
	height 40px
	line-height 40px
	font-size 16px
button 
	width 50%
	margin 0 auto
	margin-top 20px
	color textColor
	background-color lightColor
img {
	width: 100%;
	object-fit: cover;
}
</style>

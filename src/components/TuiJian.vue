<template>
	<div class="tui-jian">
		
		<div class="wntj"><p>为 你 推 荐</p></div>
		
		<div class="list left" v-for="(item,index) in nav" :key="index">
			<a href="#">
				<img class="list-img" :src="item.image" />
				<div class="list-text" v-text="item.title"></div>
				<div class="list-price" v-text="'￥'+item.price"></div>
				<button class="list-btn">看相似</button>
				
			</a>			
		</div>	
	</div>
	
</template>

<script>
	export default {

		data() {
			return {
				nav: [
					{
						title: '李宁篮球鞋 男鞋运动鞋韦德之道6队尚悟道2驭帅速雨',
						url: '#',
						image: require("@/assets/images/shoes.jpg"),
						price:1280
					},
					{
						title: '李宁篮球鞋 男鞋运动鞋韦德之道6队尚悟道2驭帅速雨',
						url: '#',
						image: require("@/assets/images/shoes.jpg"),
						price:1280
					},
					{
						title: '李宁篮球鞋 男鞋运动鞋韦德之道6队尚悟道2驭帅速雨',
						url: '#',
						image: require("@/assets/images/shoes.jpg"),
						price:1280
					},
					{
						title: '李宁篮球鞋 男鞋运动鞋韦德之道6队尚悟道2驭帅速雨',
						url: '#',
						image: require("@/assets/images/shoes.jpg"),
						price:1280
					},
					{
						title: '李宁篮球鞋 男鞋运动鞋韦德之道6队尚悟道2驭帅速雨',
						url: '#',
						image: require("@/assets/images/shoes.jpg"),
						price:1280
					},
					{
						title: '李宁篮球鞋 男鞋运动鞋韦德之道6队尚悟道2驭帅速雨',
						url: '#',
						image: require("@/assets/images/shoes.jpg"),
						price:1280
					}
						
				]
			};

		}
	}
</script>

<style lang="less">
	
	.tui-jian{
			text-align: center;
			
		.wntj{
			width:100%;
			height:0.75rem;
			background-color: white;
			
			
			p{
				font-size:0.4rem;
				font-family: "微软雅黑";
				text-align: center;
				line-height: 0.75rem;
				color: deepskyblue;
			}
		}
		
		.list{
			width:48%;
			height: auto;
			background-color: white;
			margin-left:1% ;
			margin-right:1% ;
			margin-bottom: 0.2rem;
			position: relative;
			
			.list-img{
				width: 3.52rem;
				height: 3.52rem;
				
			}
			
			.list-text{
				width:95%;
				height:0.62rem;
				padding: 0.2rem 0;
				font-size:0.26rem ;
				text-overflow: ellipsis;
			}
			.list-price{
				width:auto;
				height:0.5rem;
				text-align: left;
				line-height:0.5rem;
				padding: 0.2rem 0;
				color: red;
				
				
			}
			.list-btn{
				float:right;
				width:auto;
				height:0.4rem;
				margin: 0.2rem 0;
				position: absolute;
				right:0.2rem;
				top:4.58rem
	
			}
			
		}	
			
			
	}
	
	

</style>
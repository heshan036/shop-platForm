<template>
	<div class="leftNavWrapper">
		<h1><img src="../../static/imgs/logo.png" alt="妈妈蜜商户中心"></h1>
		<a id="publicActivity" href="javascript:">+ 发布活动</a>
		<el-menu :default-active="defaultActive" class="el-menu-vertical-demo leftMenu" @open="handleOpen" @select="handleSelect" unique-opened router>
		 	<el-menu-item index="/" class="menu_1"><i  class="iconfont icon-shouye"></i>首页</el-menu-item>
		 	<el-submenu index="2" >
		 		<template slot="title"><i class="iconfont icon-huodong"></i>活动</template>
		 		<el-menu-item index="/activity/activityList">活动列表</el-menu-item>
          		<el-menu-item index="/activity/activityPublic">活动秀</el-menu-item>
		 	</el-submenu>
		 	<el-menu-item index="/product" class="menu_1"><i  class="iconfont icon-shangpingoods"></i>商品</el-menu-item>
		 	<el-menu-item index="/validate" class="menu_1"><i  class="iconfont icon-yanzheng"></i>验证</el-menu-item>
		 	<el-submenu index="5" >
		 		<template slot="title"><i class="iconfont icon-huodong"></i>报名</template>
		 		<el-menu-item index="/signUp/list">报名列表</el-menu-item>
          		<el-menu-item index="/signUp/statistics">报名统计</el-menu-item>
		 	</el-submenu>
		 	<el-menu-item index="/order" class="menu_1"><i  class="iconfont icon-shangpingoods"></i>订单</el-menu-item>
		 	<el-menu-item index="/shop/list" class="menu_1"><i  class="iconfont icon-yanzheng"></i>门店</el-menu-item>
		 	<el-menu-item index="/merchant" class="menu_1"><i  class="iconfont icon-shangpingoods"></i>商家</el-menu-item>
		 	<el-menu-item index="/help" class="menu_1"><i  class="iconfont icon-yanzheng"></i>帮助</el-menu-item>
		</el-menu>
	</div>
</template>

<script>

export default {
	data(){
		return {
			navList:[],
			defaultActive:'/'
			//logoURL:imgPath+'logo.png'
		}
	},
	created(){
		var path=this.$route.path;
		console.log(path)
		this.defaultActive=this.$route.path;
	},
	methods:{
		handleOpen:function(index,indexPath){

		},
		handleSelect:function(index,indexPath){
			
		}
	}
}
</script>

<style>
</style>

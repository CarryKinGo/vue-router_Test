<template>
	<div id="app">
		<div class="header">
			<router-link to="/" class="nav-item">
				<img src="./assets/logo.png" />
			</router-link>
			<div class="content">
<!-- 				<router-link to="/task" class="nav-item">任务中心</router-link>
				<router-link to="/lib" class="nav-item">库管理</router-link>
				<router-link to="/ucenter" class="nav-item">流川枫</router-link> -->
        <router-link to="/home" class="nav-item">主页</router-link>
        <router-link to="/news" class="nav-item">新闻</router-link>
        <router-link to="/Myiframe/urlPath?src=https://www.google.com">iframe_URL</router-link>
<!--        <router-link to="/Myiframe/home">iframe_主页</router-link>
        <router-link to="/Myiframe/news">iframe_新闻</router-link> -->
			</div>

		</div>
		<div class=" container ">
			<router-view></router-view>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'App'
	};
</script>

<style>
	#app {
		background-color: rgb(244, 244, 244);
	}

	.header {
		display: flex;
		height: 50px;
		background-color: white;
		font-size: 20px;
		padding-left: 120px;
		align-items: center;
	}

	.nav-item {
		width: 100px;
		margin-right: 30px;
	}

	img {
		widows: 100px;
		height: 40px;
		margin-right: 100px;
	}

	.content {
		margin-left: 30%;
	}

	.container {
		width: 80%;
		margin: 0 auto;
		padding-bottom: 20px;
	}

	a {
		text-decoration: none;
		color: #aaa;
	}

	a:hover {
		color: rgb(2, 165, 218);
	}
</style>

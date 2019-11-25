<template id="iframe">
			<div>
<!-- 				<h3>urlPath : {{urlPath}}</h3>
				<h3>routerPath : {{routerPath}}</h3> -->
				<h3>src : {{$route.query.src}}</h3>
				<iframe v-if="$route.query.src" :src='$route.query.src' frameborder="0" width="1200px" height="600px"></iframe>
				<iframe v-else :src="urlPath" frameborder="0" width="1200px" height="600px"></iframe>
				<!--<iframe :src="'//elemefe.github.io/mint-ui/#'" frameborder="0" width="300px" height="300px"></iframe>-->
			</div>
		</template>
		<script>
			var Home = {
				template:"#home"
			}
			var News = {
				template:"#news"
			}
			var Details = {
				template:"#details"
			}
			var Myiframe = {
				template:"#iframe"
				,data: function() {
					return {
						msg:""
						,urlPath: this.getUrlPath() //iframe src 路径
					}
				}
				,props:['routerPath'] // 路由地址
				,watch: {
					routerPath: function(val) {// 监听routerPath变化，改变src路径
						this.urlPath = this.getUrlPath();
					}
				}
				,methods: {
					getUrlPath:function() {//获取 iframe src 路径
						let url = window.location.href;
						url = url.replace("iframe/","");
						return url;
					}
				}
			}
    </script>

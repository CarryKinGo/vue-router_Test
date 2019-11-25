<template id="details">
			<div>
				<h3>我是用户详细</h3>
				<h3>当前完整路径fullPath:{{$route.fullPath}}</h3>
				<h3>当前路径path:{{$route.path}}</h3>
				<h3>当前参数params:{{$route.params}}</h3>
				<h3>当前查询参数query:{{$route.query}}</h3>
				<h3>hash:{{$route.hash}}</h3>
				<h3>router:{{$route.router}}</h3>
				<!--<h3>matched:{{$route.matched}}</h3>-->
			</div>
		</template>
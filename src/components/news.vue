		<template id="news">
			<div>
				<div>
					<h3>我是新闻</h3>
					<router-link to="/news/details/10010?t=1">用户详细</router-link>
					<router-link to="/news/name/lucy/age/20">用户名称</router-link>
					<router-link to="/news/ret">首页</router-link>
				</div>
				<div>
					<router-view></router-view>
				</div>
			</div>
		</template>
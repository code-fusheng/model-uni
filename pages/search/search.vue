<template>
	<view>
		
		<!-- 搜索框开始 -->
		<view class="search">
			<uni-search-bar @confirm="search" @cancel="cancelInput"></uni-search-bar>
		</view>
		<!-- 搜索框结束 -->
		
		<!-- 导航菜单开始 -->
		<view class="search-navbar-container">
			<view class="navbar-item" :class="activeNavbar === item.id ? 'navbar-text-active':''" @click="changeNavbar(item.id)" v-for="item in navbarList" :key="item.id">
				<text class="navbar-text">{{item.name}}</text>
			</view>
		</view>
		<!-- 导航菜单结束 -->
		
		<!-- 文章列表开始 -->
		<article-list></article-list>
		<!-- 文章列表结束 -->
		
		<!-- 版权信息 -->
		<copyright></copyright>
		<!-- 版权信息 -->
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				// 当前选中菜单
				activeNavbar: 1,
				navbarList: [
					{id: 1, name: '发布时间'},
					{id: 2, name: '浏览量'},
					{id: 3, name: '评论数'},
					{id: 4, name: '点赞数'}
				]
			}
		},
		methods: {
			// 改变菜单项
			changeNavbar(index) {
				this.activeNavbar = index
			},
			// 
			search(e) {
				console.log(e)
				uni.navigateTo({
					url: `../search-info/search-info?searchInfo=${e.value}`
				})
			},
			// 
			cancelInput(e) {
				console.log(e)
			}
		}
	}
</script>

<style>
@import url("./index.css");
</style>

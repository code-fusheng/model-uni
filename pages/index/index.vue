<template>
	<view class="container">
		<!-- 轮播图开始 -->
		<swiper class="swiper" autoplay="true" interval="3000">
			<swiper-item>
				<view class="index-banner-container">
					<image class="index-banner" src="../../static/image/1.png" mode=""></image>
				</view>
			</swiper-item>
			<swiper-item>
				<view class="index-banner-container">
					<image class="index-banner" src="../../static/image/2.png" mode=""></image>
				</view>
			</swiper-item>
			<swiper-item>
				<view class="index-banner-container">
					<image class="index-banner" src="../../static/image/3.png" mode=""></image>
				</view>
			</swiper-item>
			<swiper-item>
				<view class="index-banner-container">
					<image class="index-banner" src="../../static/image/4.png" mode=""></image>
				</view>
			</swiper-item>
		</swiper>
		<!-- 轮播图结束 -->

		<!-- 统计数据开始 -->
		<view class="statistic-container">
			<!-- 站点访问量 -->
			<view class="statistic-user-container">
				<text class="statistic-user-text">9999</text>
				<view class="statistic-user-label-container">
					<image class="user-icon" src="../../static/icons/mine.png" mode=""></image>
					<text class="user-text">站点访问人数</text>
				</view>
			</view>
			<!-- 站点文章量 -->
			<view class="statistic-article-container">
				<text class="statistic-article-text">9999</text>
				<view class="statistic-article-label-container">
					<image class="article-icon" src="../../static/icons/wenzhang.png" mode=""></image>
					<text class="article-text">站点文章总数</text>
				</view>
			</view>
		</view>
		<!-- 数据统计结束 -->

		<!-- 系统通知公告开始 -->
		<view class="notice-container">
			<image class="notice-icon" src="../../static/icons/tongzhi.png" mode=""></image>
			<text class="notice-text">公告：欢迎来到code-fusheng的个人论坛</text>
		</view>
		<!-- 系统通知公告结束 -->

		<!-- 导航菜单开始 -->
		<scroll-view class="menu-container" scroll-x="true">
			<view :class="activeMenu === item.id ? 'menu-item menu-item-active' : 'menu-item'" v-for="item in menuList" :key="item.id" @click="clickMenu(item.id)">
				<text>{{item.name}}</text>
			</view>
		</scroll-view>
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
				// 当前默认选择
				activeMenu: 1,
				// 菜单列表
				menuList: [
					{id: 1, name: '最新发布'},
					{id: 2, name: '资源分享'},
					{id: 3, name: '技术交流'},
					{id: 4, name: '最新发布'},
					{id: 5, name: '项目实践'},
					{id: 6, name: '软件工程'},
					{id: 7, name: '数据结构'},
					{id: 8, name: '划水摸鱼'}
				]
			}
		},
		methods: {
			// 菜单点击事件
			clickMenu(index) {
				this.activeMenu = index
			}
		}
	}
</script>

<style>
	@import url("./index.css");
</style>

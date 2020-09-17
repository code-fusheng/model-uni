<template>
	<view class="">
		<view class="search-info">
			<text class="search-text">搜索关键字“{{searchInfo}}”的结果</text>
		</view>
		<!-- 文章列表 -->
		<article-list></article-list>
		<!-- 文章列表结束 -->
		
		<!-- 版权信息开始 -->
		<copyright></copyright>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				searchInfo: ''
			}
		},
		onLoad(e) {
			this.searchInfo = e.searchInfo
		}
	}
</script>

<style>
	.search-info {
		padding-left: 30rpx;
	}
	.search-text {
		font-size: 36rpx;
		line-height: 50rpx;
	}
</style>

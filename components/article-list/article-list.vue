<template>
	<view>
		<!-- 文章列表开始 -->
		<view class="article-list-container">
			<view class="article-item-container" @click="toArticleInfo(1)">
				<image class="article-image" src="../../static/springboot.jpg" mode=""></image>
				<view class="article-item">
					<view class="article-content">
						基于 Java 的个人论坛个人论坛个人论坛个人论坛个人论坛个人论坛个人论坛个人论坛个人论坛个人论坛个人论坛个人论坛个人论坛个人论坛
					</view>
					<view class="article-meta-container">
						<view class="article-meta">
							<image class="article-item-icon" src="../../static/icons/shijian.png"></image>
							<text class="article-item-text">2020/09/17</text>
						</view>
						<view class="article-meta">
							<image class="article-item-icon" src="../../static/icons/yuedu.png"></image>
							<text class="article-item-text">1</text>
						</view>
						<view class="article-meta">
							<image class="article-item-icon" src="../../static/icons/huifu.png"></image>
							<text class="article-item-text">2</text>
						</view>
						<view class="article-meta">
							<image class="article-item-icon" src="../../static/icons/dianzan.png"></image>
							<text class="article-item-text">3</text>
						</view>
					</view>
				</view>	
			</view>
		</view>
		<!-- 文章列表结束 -->
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			};
		},
		methods: {
			toArticleInfo(id) {
				uni.navigateTo({
					url: `../../pages/article-info/article-info?id=${id}`
				})
			}
		}
	}
</script>

<style>
	@import url("./article.css");
</style>

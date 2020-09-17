<template>
	<view>
		<!-- 上方标题 -->
		<view class="article-header-container">
			<view class="article-title-container">
				<view class="article-title-text">
					<text>code-fusheng 个人网站开发测试手写文章内容</text>
				</view>
				<view class="article-title-good">
					<image class="article-title-good-image" src="../../static/icons/dianzan.png" mode=""></image>
					<text class="article-title-good-text">99人赞</text>
				</view>
			</view>
			<view class="article-meta-container">
				<view class="article-meta">
					<image class="article-meta-icon" src="../../static/icons/shijian.png" mode=""></image>
					<text class="article-meta-text">2020/09/17</text>
				</view>
				<view class="article-meta">
					<image class="article-meta-icon" src="../../static/icons/yuedu.png" mode=""></image>
					<text class="article-meta-text">1</text>
				</view>
				<view class="article-meta">
					<image class="article-meta-icon" src="../../static/icons/huifu.png" mode=""></image>
					<text class="article-meta-text">1</text>
				</view>
				<view class="article-meta">
					<image class="article-meta-icon" src="../../static/icons/dianzan.png" mode=""></image>
					<text class="article-meta-text">1</text>
				</view>	
			</view>
			<view class="article-type-container">
				<uni-tag class="article-type-tag" text="#技术交流" size="small" :circle="true" type="success"></uni-tag>
			</view>
		</view>
		<!-- 分割线 -->
		<article-line></article-line>
		<!-- 上方标题结束 -->
		
		<!-- 文章内容开始 -->
		<view class="blog-conetnt">
			文章内容
		</view>
		
		<!-- 文章内容结束 -->
		
		<!-- 点赞与评论开始 -->
		<view class="article-good-container">
			<view class="article-good-title">
				99人赞
			</view>
		</view>
		
		<view class="article-comment-container">
			<view class="article-comment-title">
				评论
			</view>
			<view class="article-comment-list">
				<view class="article-comment-item">
					<view class="comment-user-name">
						code-fusheng
					</view>
					<view class="comment-content">
						忍一时越想越气、退一步越想越亏忍一时越想越气、退一步越想越亏忍一时越想越气、退一步越想越亏
						忍一时越想越气、退一步越想越亏忍一时越想越气、退一步越想越亏忍一时越想越气、退一步越想越亏
						忍一时越想越气、退一步越想越亏忍一时越想越气、退一步越想越亏忍一时越想越气、退一步越想越亏
						忍一时越想越气、退一步越想越亏忍一时越想越气、退一步越想越亏忍一时越想越气、退一步越想越亏
						忍一时越想越气、退一步越想越亏忍一时越想越气、退一步越想越亏忍一时越想越气、退一步越想越亏
					</view>
					<view class="article-time">
						5天前
					</view>
				</view>
				
				<view class="article-comment-item">
					<view class="comment-user-name">
						code-fusheng
					</view>
					<view class="comment-content">
						忍一时越想越气、退一步越想越亏
					</view>
					<view class="article-time">
						5天前
					</view>
				</view>
				
				<view class="article-comment-item">
					<view class="comment-user-name">
						code-fusheng
					</view>
					<view class="comment-content">
						忍一时越想越气、退一步越想越亏
					</view>
					<view class="article-time">
						5天前
					</view>
				</view>
			</view>
		</view>
		
		
		<!-- 点赞与评论结束 -->
		
		
		<!-- 相关阅读开始 -->
		<view class="recom-article-container">
			<view class="recom-article-title">
				相关阅读
			</view>
			<article-list></article-list>
		</view>
		<!-- 相关阅读结束 -->
		
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style>
	@import url("./index.css");
</style>

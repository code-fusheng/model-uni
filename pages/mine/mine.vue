<template>
	<view>
		<!-- 顶部背景 -->
		<view class="bg-image-container">
			<view class="header-container">
				<image class="header-image" src="../../static/code-fusheng.jpg" mode=""></image>
				<text class="user-name">浮生</text>
				<text class="header-text">code-fusheng</text>
			</view>
		</view>
		<!-- 顶部背景结束 -->
		
		
		<!-- 浮生 - 若梦 -->
		<view class="fusheng-ruomeng-container">
			<!-- 浮生 -->
			<view class="fusheng-container">
				<text class="fusheng-top-text">浮生</text>
				<text class="fusheng-buttom-text">世间繁华-何止三千</text>
			</view>
			<!-- 若梦 -->
			<view class="ruomeng-container">
				<text class="ruomeng-top-text">若梦</text>
				<text class="ruomeng-buttom-text">人生一世-何只百年</text>
			</view>
		</view>
		<!-- 结束 -->
		
		<!-- 菜单开始 -->
			<view class="mine-menu-container">
				<uni-list class="menu-container">
					<uni-list-item title="分享好友" thumb="/static/icons/fenxianghaoyou.png"></uni-list-item>
					<uni-list-item title="赞赏支持" thumb="/static/icons/zanshangzhichi.png"></uni-list-item>
					<uni-list-item title="时间轴" thumb="/static/icons/shijian.png"></uni-list-item>
					<uni-list-item title="意见反馈" thumb="/static/icons/yijianfankui.png"></uni-list-item>
					<uni-list-item title="联系客服" thumb="/static/icons/lianxikefu.png"></uni-list-item>
					<uni-list-item title="关于我们" thumb="/static/icons/guanyuwomen.png"></uni-list-item>
				</uni-list>
			</view>
		<!-- 菜单结束 -->
		
		<!-- 版权信息 -->
		<copyright></copyright>
		<!-- 版权信息 -->
		
		
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

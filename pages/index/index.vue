<template>
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view class="text-area">
			<text class="title">{{title}}</text>
			
		</view>
		<navigator  url="viewcontainer/view">
			<button type="default">视图组件</button>
		</navigator>
	</view>
</template>

<script>
	export default {
		data() {
			return {
            title:"点击进入对应组件界面"
			}
		},
		onLoad(option) {
			console.log(option.id);
			console.log(option.name);
		},
		methods: {

		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>

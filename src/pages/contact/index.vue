<template>
	<view class="content">
		<view>
            <section class="section">
                <text>{{contacts}}</text>
            </section>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
                contacts: `
					微信：tychio
					Email: work@tychio.net		
				`
			}
		},
		onLoad() {

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
    .section {
        text-indent: 30px;
        padding: 30px 20px 0px;
    }
</style>

<template>
	<view class="content">
		<view>
            <section class="section" v-for="intro, index in intros" :key={index}>
                <text>{{intro.text}}</text>
            </section>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
                intros: [
                    {
                        text: '张铮铮，资深全栈程序员，Web前端开发者，高级软件咨询师'
                    },
                    {
                        text: '曾就职于知名软件咨询公司，经历过多个创业公司，有丰富的项目启动和落地经验。'
                    },
                    {
                        text: '善于深度挖掘产品需求，切合客户利益提出解决方案，并高效准确的完成开发。'
                    }
                ] 
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

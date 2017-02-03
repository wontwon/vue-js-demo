<template>
	<div>
		<h5>Bye Bye</h5>
		<div>This is some random ass text</div>
		<div v-for="name in groupNames">
			<div @click="runThisFunction">{{ name }}</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'ByeBye',
		props: ["groupNames"],
		methods: {
			runThisFunction() {
				console.log("your mama")
			}
		},
		created() {
		  console.log("Bye Bye component just got created")
		}
	}
</script>


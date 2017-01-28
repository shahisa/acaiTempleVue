<template>
	<div class="Hello__Wrapper">
		<hello-header class="Hello__HelloHeader--background"></hello-header>
	</div>
</template>

<script type="text/javascript">
	import HelloHeader from './HelloHeader';

	export default {
		name: 'Hello',
		components: {
			HelloHeader,
		},
	};
</script>

<style type="text/css">
	.Hello__HelloHeader--background {
		background: url(../../assets/img/bg-pattern.png),#7b4397;
        background: url(../../assets/img/bg-pattern.png),-webkit-linear-gradient(to left,#7b4397,#dc2430);
        background: url(../../assets/img/bg-pattern.png),linear-gradient(to left,#7b4397,#dc2430);
        padding: 0 2em;
	}
</style>
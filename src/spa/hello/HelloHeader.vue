<template>
	<header class="HelloHeader__Header">
        <md-layout>
            <md-layout>
                <div class="HelloHeader__Description">
                    <h1 class="HelloHeader__DescriptionHeader--spacing">
                        Açaí will allow you to start a crowdsource borrowing campaign, loan money, or invest in the stock market.
                    </h1>
                    <md-button class="md-raised md-accent">
                        Start Now for Free!
                    </md-button>
                </div>
            </md-layout>
            <md-layout>
                <div>
                    <img src="img/demo-screen-1.jpg" alt="">
                </div>
                <div class="button">
                </div>
            </md-layout>
        </md-layout>
    </header>
</template>

<script type="text/javascript">
	export default {
		name: 'HelloHeader',
	};
</script>

<style type="text/css">
    .HelloHeader__Header {
        position: relative;
        height: 90vh;
        width: 100%;
        min-height: auto;
        overflow-y: hidden;
        color: #fff;
    }

    .HelloHeader__Description {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        align-content: center;
        height: 90vh;
    }

    .HelloHeader__DescriptionHeader--spacing {
        line-height: 1.2em;
    }
</style>
<template>
	<div class="dashboard-template" data-app>
		<div class="d-dashboard-header">
			<div class="d-dashboard-header-left">
				<div class="d-head-logo"><img src="@/assets/images/logo_black.png"/></div>
				<div class="d-head-mid">X</div>
				<div class="d-head-departmnet">Moneybacker$</div>
			</div>
			<div class="d-dashboard-header-right">
				<div class="d-header-menu">
					<ul>
						<li>Attendance</li>
						<li>Tickets</li>
					</ul>
				</div>
			</div>
		</div>
		<div class="d-dashboard-content">
			<Nuxt />
		</div>
	</div>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {
    }
  }
}
</script>

<style scoped>

	.d-dashboard-header {
		background: #fff;
		box-shadow: 0 0 12px #ccc;
		padding: 20px 35px;
		margin-bottom: 30px;
	}
	
	.d-dashboard-content {
		width: 80%;
		margin: 0 auto;
	}
</style>

<style>
	body {
		background: #fafafa;
		font-family: 'Roboto Condensed', sans-serif;
	}
	.d-section-header {
		text-align: center;
		margin-bottom: 35px;
	}
	.d-section-header > span {
		background: #fff;
		font-size: 50px;
		text-transform: capitalize;
		font-weight: 700;
		padding: 0 20px;
		font-family: 'Covered By Your Grace', cursive;
		color: #4a4a4a;
	}
	.d-section-header > hr {
		margin-top: -35px;
	}
	.d-dashboard-header img {
		width: 250px;
	}

	.d-dashboard-header-left > div {
		display: inline-block;
		vertical-align: middle;
	}
	.d-head-departmnet {
		font-size: 31px;
		text-transform: uppercase;
		font-weight: 100;
	}
	.d-head-mid {
		padding: 0 10px;
		font-size: 42px;
		line-height: 1em;
		font-weight: 100;
	}

	.d-dashboard-header-left {
		display: inline-block;
		vertical-align: middle;
		width: 30%;
	}
	.d-dashboard-header-right {
		display: inline-block;
		vertical-align: middle;
		width: 68%;
		text-align: right;
	}

	.d-header-menu ul {
		margin: 0;
		padding: 0;
	}
	.d-header-menu ul li {
		display: inline-block;
		background: #333;
		color: #fff;
		line-height: 1em;
		font-size: 16px;
		padding: 15px 25px;
		border-radius: 50px;
		cursor: pointer;
	}
</style>
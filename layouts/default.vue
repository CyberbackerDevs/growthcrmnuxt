<template>
	<div>
		<!--begin::Main-->
		<!--begin::Root-->
		<div class="d-flex flex-column flex-root">
			<!--begin::Page-->
			<div class="page d-flex flex-row flex-column-fluid">
				<!--begin::Aside-->
				<segmentsMenu />
				<!--end::Aside-->
				<!--begin::Wrapper-->
				<div class="wrapper d-flex flex-column flex-row-fluid" id="kt_wrapper">
					<!--begin::Header tablet and mobile-->
					<div class="header-mobile py-3">
						<!--begin::Container-->
						<div class="container d-flex flex-stack">
							<!--begin::Mobile logo-->
							<div class="d-flex align-items-center flex-grow-1 flex-lg-grow-0">
								<a href="#">
									<img alt="Logo" src="@/assets/media/logos/logo-demo9.svg" class="h-35px" />
								</a>
							</div>
							<!--end::Mobile logo-->
							<!--begin::Aside toggle-->
							<button class="btn btn-icon btn-active-color-primary" id="kt_aside_toggle">
								<!--begin::Svg Icon | path: icons/duotune/abstract/abs015.svg-->
								<span class="svg-icon svg-icon-2x me-n1">
									<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
										<path d="M21 7H3C2.4 7 2 6.6 2 6V4C2 3.4 2.4 3 3 3H21C21.6 3 22 3.4 22 4V6C22 6.6 21.6 7 21 7Z" fill="black" />
										<path opacity="0.3" d="M21 14H3C2.4 14 2 13.6 2 13V11C2 10.4 2.4 10 3 10H21C21.6 10 22 10.4 22 11V13C22 13.6 21.6 14 21 14ZM22 20V18C22 17.4 21.6 17 21 17H3C2.4 17 2 17.4 2 18V20C2 20.6 2.4 21 3 21H21C21.6 21 22 20.6 22 20Z" fill="black" />
									</svg>
								</span>
								<!--end::Svg Icon-->
							</button>
							<!--end::Aside toggle-->
						</div>
						<!--end::Container-->
					</div>
					<!--end::Header tablet and mobile-->
					<!--begin::Header-->
					<segmentsHeader />
					<!--end::Header-->
					<!--begin::Content-->
					<div class="content d-flex flex-column flex-column-fluid" id="kt_content">
						<!--begin::Container-->
						<div class="container-xxl" id="kt_content_container">
							<!--begin::Row-->
							<Nuxt />
							<!--end::Row-->
						</div>
						<!--end::Container-->
					</div>
					<!--end::Content-->
					<!--begin::Footer-->
					<SegmentsFooter />
					<!--end::Footer-->
				</div>
				<!--end::Wrapper-->
			</div>
			<!--end::Page-->
		</div>
		<!--end::Root-->
		<!--end::Scrolltop-->
		<SegmentsScripts />
		<!--end::Javascript-->
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
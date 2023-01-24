<template>
	<div class="d-dashboard-main">
		<div class="d-main-content">
			<div class="row d-main-content-inner">
				<div class="col-xl-4 d-left-part">
					<DashboardMentions />
					<DashboardTickets />
				</div>
				<div class="col-xl-8 ps-xl-12 d-right-part">
					<div class="card bgi-position-y-bottom bgi-position-x-end bgi-no-repeat bgi-size-cover min-h-250px bg-primary mb-5 mb-xl-8 surprise_dashboard" style="">
						<!--begin::Body-->
						<div class="card-body d-flex flex-column justify-content-center">
							<!--begin::Title-->
							<h3 class="text-white fs-2x fw-bolder line-height-lg mb-5">Hi Arphie!
							<br />Start your day with a bang!</h3>
							<!--end::Title-->
							<!--begin::Action-->
							<!-- <div class="m-0">
								<a href='#' class="btn btn-success fw-bold px-6 py-3" data-bs-toggle="modal" data-bs-target="#kt_modal_create_app">Create an App</a>
							</div> -->
							<!--begin::Action-->
						</div>
						<!--end::Body-->
					</div>
					<div class="row g-5 g-xl-8">
						<dashboardBigStats />
						<DashboardPto />
						<DashboardPrepay />
					</div>
				</div>
			</div>

		</div>
	</div>
</template>

<script>
    export default {
        name: 'mbdashboard',
        data () {
            return {
				
            }
        },
        methods: {
			
        }
    }
</script>

<style scoped>
	/* .d-main-content {
        background: #fff;
        padding: 10px;
        border-radius: 5px;
        box-shadow: 0 0 12px #efefef;
    } */
	.surprise_dashboard {
		background-position: 100% 50px;
		background-size: 500px auto;
		background-image:url('~@/assets/media/misc/city.png')
	}
</style>
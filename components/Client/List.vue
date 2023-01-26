<template>
    <div>
        <div class="row g-5 g-xl-10 mb-xl-10">
            <div class="col-md-3 col-lg-3 col-xl-3 col-xxl-3 mb-md-5 mb-xl-10">
                <div class="card bgi-position-y-bottom bgi-position-x-end bgi-no-repeat bgi-size-cover min-h-250px mb-5 mb-xl-8 bg-light-warning surprise_dashboard" style="">
                    <!--begin::Body-->
                    <div class="card-body d-flex flex-column justify-content-center">
                        <!--begin::Title-->
                        <h3 class="text-dark fs-2x fw-bolder line-height-lg mb-5">Open the
                        <br />Client Masterlist</h3>
                        <!--end::Title-->
                        <!--begin::Action-->
                        <div class="m-0">
                            <a href='#' class="btn btn-light-primary fw-bold px-6 py-3" data-bs-toggle="modal" data-bs-target="#kt_modal_create_app">Open List</a>
                        </div>
                        <!--begin::Action-->
                    </div>
                    <!--end::Body-->
                </div>
            </div>

            <div class="col-md-3 col-lg-3 col-xl-3 col-xxl-3 mb-md-5 mb-xl-10">
                <div class="card bgi-position-y-bottom bgi-position-x-end bgi-no-repeat bgi-size-cover min-h-250px mb-5 mb-xl-8 bg-light-primary surprise_dashboard" style="">
                    <!--begin::Body-->
                    <div class="card-body d-flex flex-column justify-content-center">
                        <!--begin::Title-->
                        <h3 class="text-dark fs-2x fw-bolder line-height-lg mb-5">Open the
                        <br />Leads List</h3>
                        <!--end::Title-->
                        <!--begin::Action-->
                        <div class="m-0">
                            <a href='#' class="btn btn-light-primary fw-bold px-6 py-3" data-bs-toggle="modal" data-bs-target="#kt_modal_create_app">Open List</a>
                        </div>
                        <!--begin::Action-->
                    </div>
                    <!--end::Body-->
                </div>
            </div>

            <div class="col-md-3 col-lg-3 col-xl-3 col-xxl-3 mb-md-5 mb-xl-10">
                <div class="card bgi-position-y-bottom bgi-position-x-end bgi-no-repeat bgi-size-cover min-h-250px mb-5 mb-xl-8 bg-light-danger surprise_dashboard" style="">
                    <!--begin::Body-->
                    <div class="card-body d-flex flex-column justify-content-center">
                        <!--begin::Title-->
                        <h3 class="text-dark fs-2x fw-bolder line-height-lg mb-5">Open the
                        <br />Bussiness Evaluation</h3>
                        <!--end::Title-->
                        <!--begin::Action-->
                        <div class="m-0">
                            <a href='#' class="btn btn-light-primary fw-bold px-6 py-3" data-bs-toggle="modal" data-bs-target="#kt_modal_create_app">Open List</a>
                        </div>
                        <!--begin::Action-->
                    </div>
                    <!--end::Body-->
                </div>
            </div>

            <div class="col-md-3 col-lg-3 col-xl-3 col-xxl-3 mb-md-5 mb-xl-10">
                <div class="card bgi-position-y-bottom bgi-position-x-end bgi-no-repeat bgi-size-cover min-h-250px mb-5 mb-xl-8 bg-light-secondary surprise_dashboard" style="">
                    <!--begin::Body-->
                    <div class="card-body d-flex flex-column justify-content-center">
                        <!--begin::Title-->
                        <h3 class="text-dark fs-2x fw-bolder line-height-lg mb-5">Open the
                        <br />For Pairing</h3>
                        <!--end::Title-->
                        <!--begin::Action-->
                        <div class="m-0">
                            <a href='#' class="btn btn-light-primary fw-bold px-6 py-3" data-bs-toggle="modal" data-bs-target="#kt_modal_create_app">Open List</a>
                        </div>
                        <!--begin::Action-->
                    </div>
                    <!--end::Body-->
                </div>
            </div>
        </div>
        
        <div class="card ">
            <!--begin::Card body-->
            <div class="card-body p-0">
                <!--begin::Wrapper-->
                <div class="card-px text-center py-20 my-10">
                    <!--begin::Title-->
                    <h2 class="fs-2x fw-bold mb-10">Search for Clients Info</h2>
                    <!--end::Title-->

                    <!--begin::Description-->
                    <p class="text-gray-400 fs-4 fw-semibold mb-10">
                        <div class="mb-10">
                            <label for="exampleFormControlInput1" class="required form-label">Example</label>
                            <input type="email" class="form-control form-control-solid" placeholder="Example input"/>
                        </div>
                    </p>
                    <!--end::Description-->

                    <!--begin::Action-->
                    <a href="#" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#kt_modal_add_customer">Add Customer</a>
                    <!--end::Action-->
                </div>
                <!--end::Wrapper-->

                <!--begin::Illustration-->
                <div class="text-center px-4">
                    <img class="mw-100 mh-300px" alt="" src="@/assets/media/illustrations/sigma-1/2.png">
                </div>
                <!--end::Illustration-->
            </div>
            <!--end::Card body-->
        </div>
    </div>
</template>

<style scoped>

	.surprise_dashboard::before {
        content: "";
		background-position: 100% 50px;
		background-size: 500px auto;
		background-image:url('~@/assets/media/misc/city.png');
        background-size: cover;
        position: absolute;
        top: 0px;
        right: 0px;
        bottom: 0px;
        left: 0px;
        opacity: 0.3;
        z-index: 1;
	}

    .surprise_dashboard .card-body {
        z-index: 2;
    }
</style>
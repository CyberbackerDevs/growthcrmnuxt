<template>
    <div class="row g-5 g-xl-8">
        <div class="col-xl-8">
            <div class="card bgi-position-y-bottom bgi-position-x-end bgi-no-repeat bgi-size-cover min-h-250px mb-5 mb-xl-8 bg-warning surprise_dashboard" style="">
                <!--begin::Body-->
                <div class="card-body d-flex flex-column justify-content-center">
                    <!--begin::Title-->
                    <h3 class="text-white fs-2x fw-bolder line-height-lg mb-5">Hi Some Agent!
                    <br />Schedule a Business Evaluation</h3>
                    <!--end::Title-->
                    <!--begin::Action-->
                    <div class="m-0">
                        <a href='#' class="btn btn-danger fw-bold px-6 py-3" data-bs-toggle="modal" data-bs-target="#kt_modal_create_app">Check the Roadmap</a>
                    </div>
                    <!--begin::Action-->
                </div>
                <!--end::Body-->
            </div>

            <div class="card mb-5 mb-xl-8">
                <!--begin::Header-->
                    <div class="card-header align-items-center border-0 mt-4">
                        <h3 class="card-title align-items-start flex-column">
                            <span class="fw-bold mb-2 text-dark">History</span>            
                            <!-- <span class="text-muted fw-semibold fs-7">890,344 Sales</span> -->
                        </h3>
                    </div>
                <!--end::Header-->

                    <!--begin::Body-->
                <div class="card-body pt-5">
                    <!--begin::Timeline-->
                    <div class="timeline-label">
                        <!--begin::Item-->
                        <div class="timeline-item">
                            <!--begin::Label-->
                            <div class="timeline-label fw-bold text-gray-800 fs-6">01</div>
                            <!--end::Label-->

                            <!--begin::Badge-->
                            <div class="timeline-badge">
                                <i class="fa fa-genderless text-warning fs-1"></i>
                            </div>
                            <!--end::Badge-->

                            <!--begin::Text-->
                            <div class="timeline-content d-flex">
                                <div class="flex-grow-1 me-2">
                                    <a href="#" class="text-gray-800 text-hover-primary fs-6 fw-bold">Outlines keep you honest. And keep structure</a>
                                    <span class="text-muted fw-semibold d-block fs-7">January 22, 2023</span>
                                </div>
                            </div>
                            <!--end::Text-->
                        </div>
                        <!--end::Item-->

                        <!--begin::Item-->
                        <div class="timeline-item">
                            <!--begin::Label-->
                            <div class="timeline-label fw-bold text-gray-800 fs-6">02</div>
                            <!--end::Label-->

                            <!--begin::Badge-->
                            <div class="timeline-badge">
                                <i class="fa fa-genderless text-success fs-1"></i>
                            </div>
                            <!--end::Badge-->

                            <!--begin::Content-->
                            <div class="timeline-content d-flex">
                                <div class="flex-grow-1 me-2">
                                    <a href="#" class="text-gray-800 text-hover-primary fs-6 fw-bold">Outlines keep you honest. And keep structure</a>
                                    <span class="text-muted fw-semibold d-block fs-7">January 22, 2023</span>
                                </div>
                            </div>
                            <!--end::Content-->
                        </div>
                        <!--end::Item-->
                    </div>
                    <!--end::Timeline-->
                </div>
                <!--end: Card Body-->
            </div>
        </div>
        <div class="col-xl-4 ps-xl-12">
            <div class="card card-flush" style="margin-bottom: 25px;">  
                <!--begin::Body-->
                <div class="card-body text-center pb-5"> 
                    <!--begin::Overlay-->
                    <div class="d-image d-agent-image">
                        <img src="@/assets/media/avatars/150-24.jpg" alt="image" />
                    </div>
                    <!--end::Overlay-->          

                    <!--begin::Info-->
                    <div class="align-items-end flex-stack mb-1">             
                       <div class="text-gray-800 text-hover-primary fs-1 d-block fw-bold agent_name">John Peter Doe</div>
                       <div class="text-gray-400 fs-7 fw-bold me-2 d-block lh-1 pb-1">Growth Backer</div>
                    </div> 
                    <!--end::Info-->   
                </div>
                <!--end::Body-->
            </div>

            <div class="card card-flush" style="margin-bottom: 25px;">  
                <!--begin::Body-->
                <div class="card-body text-center pb-5"> 
                    <!--begin::Overlay-->
                    <div class="d-image d-agent-image">
                        <img src="@/assets/media/avatars/150-24.jpg" alt="image" />
                    </div>
                    <!--end::Overlay-->          

                    <!--begin::Info-->
                    <div class="align-items-end flex-stack mb-1">             
                       <div class="text-gray-800 text-hover-primary fs-1 d-block fw-bold agent_name">Some Agent Name</div>
                       <div class="text-gray-400 fs-7 fw-bold me-2 d-block lh-1 pb-1">Lead Backer</div>
                    </div> 
                    <!--end::Info-->   
                </div>
                <!--end::Body-->
            </div>


            
        </div>
    </div>
</template>

<style scoped>

	.surprise_dashboard {
		background-position: 100% 50px;
		background-size: 500px auto;
		background-image:url('~@/assets/media/misc/city.png')
	}

    .agent_name {
        margin-top: 15px;
    }

    .d-image.d-agent-image img {
        width: 84%;
        display: block;
        border-radius: 10px;
        margin: 0 auto;
    }
</style>
<template>
    <!--begin::Timeline content-->
    <div class="timeline-content mb-10 mt-n1">
        <!--begin::Timeline heading-->
        <div class="pe-3 mb-5">
            <!--begin::Title-->
            <div class="fs-5 fw-semibold mb-2">Assign client to Growth Backer</div>
            <!--end::Title-->
            <!--begin::Description-->
            <div class="d-flex align-items-center mt-1 fs-6"><div class="text-muted me-2 fs-7">Added at 4:23 PM by Arphie Balboa</div></div>
            <!--end::Description-->
        </div>
        <!--end::Timeline heading-->

        <!--begin::Timeline details-->
        <div class="overflow-auto pb-5">

            <div class="alert alert-dismissible bg-light-info border border-info d-flex flex-column flex-sm-row w-100 p-5 mb-10">
                <div class="timeline-icon symbol symbol-circle symbol-50px me-4 mb-5 mb-sm-0">
                    <div class="symbol-label bg-info">
                        <i class="bi bi-person-bounding-box fs-2x text-white"></i>
                    </div>
                </div>
                <div class="d-flex flex-column pe-0 pe-sm-10">
                    <h5 class="mb-1">John Peter Doe has been selected as a Growthbacker for the client</h5>
                    <span>Has been executed by Sample person on January 12, 2023</span>
                </div>
                <button type="button" class="position-absolute position-md-relative m-2 w-250px m-sm-0 top-0 end-0 btn btn-info text-white ms-sm-auto">
                    Change Growthbacker
                </button>
            </div>

            <!--begin::Alert-->
            <div class="alert alert-dismissible bg-light-primary d-flex flex-center flex-column py-10 px-10 px-lg-20 mb-10">

                <!--begin::Icon-->
                <div class="timeline-icon symbol symbol-circle symbol-60px me-4">
                    <div class="symbol-label bg-primary">
                        <i class="bi bi-person fs-3x text-white"></i>
                    </div>
                </div>
                <!--end::Icon-->

                <!--begin::Wrapper-->
                <div class="text-center w-75" style="margin-top: 20px;">
                    <!--begin::Title-->
                    <!-- <h1 class="fw-bolder mb-5">Assign a Lead backer to</h1> -->
                    <!--end::Title-->

                    <!--begin::Separator-->
                    <div class="separator separator-dashed border-danger opacity-25 mb-5"></div>
                    <!--end::Separator-->

                    <!--begin::Content-->
                    <div class="mb-9 text-dark">
                        Assign a lead backer to the client
                    </div>
                    <!--end::Content-->

                    <div class="of-form">
                        <div class="mb-10">
                            <select class="form-select" aria-label="Select example">
                                <option>Open this select menu</option>
                                <option value="1">One</option>
                                <option value="2">Two</option>
                                <option value="3">Three</option>
                            </select>
                        </div>
                    </div>

                    <!--begin::Buttons-->
                    <div class="d-flex flex-center flex-wrap">
                        <!-- <a href="#" class="btn btn-outline btn-outline-primary btn-active-primary m-2">Cancel</a> -->
                        <a href="#" class="btn btn-success m-2">Ok, I got it</a>
                    </div>
                    <!--end::Buttons-->
                </div>
                <!--end::Wrapper-->
            </div>
            <!--end::Alert-->
        </div>
        <!--end::Timeline details-->
    </div>
    <!--end::Timeline content-->
</template>
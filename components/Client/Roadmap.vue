<template>
    <div class="d-road-map-flow">
        <div class="d-main-content current_roadmap">
            <div class="d-flex flex-wrap flex-stack my-5">
                <!--begin::Heading-->
                <h2 class="fs-2 fw-semibold my-2">Current Roadmap 
                <span class="fs-6 text-gray-400 ms-1">last updated on January 18, 2023</span></h2>
                <!--end::Heading-->
                <!--begin::Controls-->
            </div>
        </div>

        <div class="d-main-container">
            <div class="card mb-8">
                <div class="card-body pt-9 pb-0">
                    <div class="timeline">
                        <!--begin::Timeline item-->
                        <div class="timeline-item"><!--  Assign to Lead Backer -->
                            <!--begin::Timeline line-->
                            <div class="timeline-line w-40px"></div>
                            <!--end::Timeline line-->

                            <!--begin::Timeline icon-->
                            <div class="timeline-icon symbol symbol-circle symbol-60px me-4">
                                <div class="symbol-label bg-success">
                                    <i class="bi bi-check2-circle fs-2 text-white"></i>
                                </div>
                            </div>
                            <!--end::Timeline icon-->

                            <RoadmapAssignLeads />  
                        </div>
                        
                        <div class="timeline-item"> <!--  Assign to Growth Backer -->
                            <!--begin::Timeline line-->
                            <div class="timeline-line w-40px"></div>
                            <!--end::Timeline line-->

                            <!--begin::Timeline icon-->
                            <div class="timeline-icon symbol symbol-circle symbol-60px me-4">
                                <div class="symbol-label bg-primary">
                                    <i class="bi bi-pencil-fill fs-2 text-white"></i>
                                </div>
                            </div>
                            <!--end::Timeline icon-->

                            <RoadmapAssignGrowth />    
                        </div>

                        <div class="timeline-item"> <!--  Business Evaluation -->
                            <!--begin::Timeline line-->
                            <div class="timeline-line w-40px"></div>
                            <!--end::Timeline line-->

                            <!--begin::Timeline icon-->
                            <div class="timeline-icon symbol symbol-circle symbol-60px me-4">
                                <div class="symbol-label bg-secondary">
                                    <i class="bi bi-lock-fill fs-2"></i>
                                </div>
                            </div>
                            <!--end::Timeline icon-->

                            <RoadmapBe />
                        </div>

                        <div class="timeline-item"> <!--  Service Agreement -->
                            <!--begin::Timeline line-->
                            <div class="timeline-line w-40px"></div>
                            <!--end::Timeline line-->

                            <!--begin::Timeline icon-->
                            <div class="timeline-icon symbol symbol-circle symbol-60px me-4">
                                <div class="symbol-label bg-secondary">
                                    <i class="bi bi-lock-fill fs-2"></i>
                                </div>
                            </div>
                            <!--end::Timeline icon-->

                            <RoadmapServiceAgreement />
                        </div>

                        <div class="timeline-item"> <!--  Introduction to Career Team -->
                            <!--begin::Timeline line-->
                            <div class="timeline-line w-40px"></div>
                            <!--end::Timeline line-->

                            <!--begin::Timeline icon-->
                            <div class="timeline-icon symbol symbol-circle symbol-60px me-4">
                                <div class="symbol-label bg-secondary">
                                    <i class="bi bi-lock-fill fs-2"></i>
                                </div>
                            </div>
                            <!--end::Timeline icon-->

                            <RoadmapIntoToCareer />
                        </div>

                        <div class="timeline-item"> <!--  Setup fee -->
                            <!--begin::Timeline line-->
                            <div class="timeline-line w-40px"></div>
                            <!--end::Timeline line-->

                            <!--begin::Timeline icon-->
                            <div class="timeline-icon symbol symbol-circle symbol-60px me-4">
                                <div class="symbol-label bg-secondary">
                                    <i class="bi bi-lock-fill fs-2"></i>
                                </div>
                            </div>
                            <!--end::Timeline icon-->

                            
                            <RoadmapSetupFee />
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'RoadMap',
        data () {
            return {
				
            }
        },
        methods: {
			
        }
    }
</script>
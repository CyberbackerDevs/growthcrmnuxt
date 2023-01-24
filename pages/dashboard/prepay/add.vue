<template>
    <div>
        <div class="d-pform-header">
            <div class="card mb-5 mb-xxl-8">
                <div class="card-body pt-9 pb-0">
                    <!--begin::Details-->
                    <div class="d-flex flex-wrap flex-sm-nowrap">
                        <!--begin: Pic-->
                        <div class="me-7 mb-4">
                            <div class="symbol symbol-100px symbol-lg-160px symbol-fixed position-relative">
                                <img src="@/assets/media/avatars/150-26.jpg" alt="image">
                                <div class="position-absolute translate-middle bottom-0 start-100 mb-6 bg-success rounded-circle border border-4 border-body h-20px w-20px"></div>
                            </div>
                        </div>
                        <!--end::Pic-->
                        <!--begin::Info-->
                        <div class="flex-grow-1">
                            <!--begin::Title-->
                            <div class="d-flex justify-content-between align-items-start flex-wrap mb-2">
                                <!--begin::User-->
                                <div class="d-flex flex-column">
                                    <!--begin::Name-->
                                    <div class="d-flex align-items-center mb-2">
                                        <a href="#">
                                            <!--begin::Svg Icon | path: icons/duotune/general/gen026.svg-->
                                            <span class="svg-icon svg-icon-1 svg-icon-primary">
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" viewBox="0 0 24 24">
                                                    <path d="M10.0813 3.7242C10.8849 2.16438 13.1151 2.16438 13.9187 3.7242V3.7242C14.4016 4.66147 15.4909 5.1127 16.4951 4.79139V4.79139C18.1663 4.25668 19.7433 5.83365 19.2086 7.50485V7.50485C18.8873 8.50905 19.3385 9.59842 20.2758 10.0813V10.0813C21.8356 10.8849 21.8356 13.1151 20.2758 13.9187V13.9187C19.3385 14.4016 18.8873 15.491 19.2086 16.4951V16.4951C19.7433 18.1663 18.1663 19.7433 16.4951 19.2086V19.2086C15.491 18.8873 14.4016 19.3385 13.9187 20.2758V20.2758C13.1151 21.8356 10.8849 21.8356 10.0813 20.2758V20.2758C9.59842 19.3385 8.50905 18.8873 7.50485 19.2086V19.2086C5.83365 19.7433 4.25668 18.1663 4.79139 16.4951V16.4951C5.1127 15.491 4.66147 14.4016 3.7242 13.9187V13.9187C2.16438 13.1151 2.16438 10.8849 3.7242 10.0813V10.0813C4.66147 9.59842 5.1127 8.50905 4.79139 7.50485V7.50485C4.25668 5.83365 5.83365 4.25668 7.50485 4.79139V4.79139C8.50905 5.1127 9.59842 4.66147 10.0813 3.7242V3.7242Z" fill="currentColor"></path>
                                                    <path d="M14.8563 9.1903C15.0606 8.94984 15.3771 8.9385 15.6175 9.14289C15.858 9.34728 15.8229 9.66433 15.6185 9.9048L11.863 14.6558C11.6554 14.9001 11.2876 14.9258 11.048 14.7128L8.47656 12.4271C8.24068 12.2174 8.21944 11.8563 8.42911 11.6204C8.63877 11.3845 8.99996 11.3633 9.23583 11.5729L11.3706 13.4705L14.8563 9.1903Z" fill="white"></path>
                                                </svg>
                                            </span>
                                            <!--end::Svg Icon-->
                                        </a>
                                        <input placeholder="Enter Form title"/>
                                    </div>
                                    <!--end::Name-->
                                    <!--begin::Info-->
                                    <div class="d-flex flex-wrap fw-semibold fs-6 mb-4 pe-2">
                                        <!--begin::Svg Icon | path: icons/duotune/communication/com006.svg-->
                                        <span class="svg-icon svg-icon-4 me-1">
                                            <svg width="18" height="18" viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
                                                <path opacity="0.3" d="M16.5 9C16.5 13.125 13.125 16.5 9 16.5C4.875 16.5 1.5 13.125 1.5 9C1.5 4.875 4.875 1.5 9 1.5C13.125 1.5 16.5 4.875 16.5 9Z" fill="currentColor"></path>
                                                <path d="M9 16.5C10.95 16.5 12.75 15.75 14.025 14.55C13.425 12.675 11.4 11.25 9 11.25C6.6 11.25 4.57499 12.675 3.97499 14.55C5.24999 15.75 7.05 16.5 9 16.5Z" fill="currentColor"></path>
                                                <rect x="7" y="6" width="4" height="4" rx="2" fill="currentColor"></rect>
                                            </svg>
                                        </span> Please add an Appropriate Title for the Form
                                    </div>
                                    <!--end::Info-->
                                </div>
                                <!--end::User-->
                                <!--begin::Actions-->
                                <div class="d-flex my-4">
                                    <a href="#" class="btn btn-sm btn-light me-2">Cancel</a>
                                    <a href="#" class="btn btn-sm btn-primary me-2" >Save</a>
                                    <!--begin::Menu-->
                                    <!--end::Menu-->
                                </div>
                                <!--end::Actions-->
                            </div>
                            <!--end::Title-->
                            <!--begin::Stats-->
                            <div class="d-flex flex-wrap flex-stack">
                                <!--begin::Wrapper-->
                                <div class="d-flex flex-column flex-grow-1 pe-8">
                                    <!--begin::Stats-->
                                    <div class="d-flex flex-wrap">
                                        <!--begin::Stat-->
                                        <div class="border border-gray-300 border-dashed rounded min-w-125px py-3 px-4 me-6 mb-3">
                                            <!--begin::Number-->
                                            <select class="form-select form-select-solid" aria-label="Select example">
                                                <option value="1">Division One</option>
                                                <option value="2">Division Two</option>
                                                <option value="3">Division Three</option>
                                            </select>
                                            <!--end::Number-->
                                            <!--begin::Label-->
                                            <div class="fw-semibold fs-6 text-gray-400">Please Choose a Division</div>
                                            <!--end::Label-->
                                        </div>
                                        <!--end::Stat-->
                                    </div>
                                    <!--end::Stats-->
                                </div>
                                <!--end::Wrapper-->
                            </div>
                            <!--end::Stats-->
                        </div>
                        <!--end::Info-->
                    </div>
                    <!--end::Details-->
                    <!--begin::Navs-->
                    <!--begin::Navs-->
                </div>
            </div>
        </div>
        <div class="d-add-form-options" v-if="prepay_id > 0">
            <div class="d-flex flex-wrap flex-stack pt-10 pb-8">
                <!--begin::Heading-->
                <h3 class="fw-bold my-2">Build New Form
                <span class="fs-6 text-gray-400 fw-semibold ms-1">Max of 3 Pages</span></h3>
                <!--end::Heading-->
                <!--begin::Controls-->
                <!--end::Controls-->
            </div>
        </div>
        <div class="d-Dform-info" v-if="prepay_id > 0">
            <div id="kt_project_targets_card_pane" class="tab-pane fade show active" role="tabpanel">
                <!--begin::Row-->
                <div class="row g-9">
                    <!--begin::Col-->
                    <div class="col-md-4 col-lg-12 col-xl-4">
                        <!--begin::Col header-->
                        <div class="mb-9">
                            <div class="d-flex flex-stack">
                                <div class="fw-bold fs-4">Page 1 
                                <span class="fs-6 text-gray-400 ms-2">0</span></div>
                                <!--begin::Menu-->
                                <!--end::Menu-->
                            </div>
                            <div class="h-3px w-100 bg-warning"></div>
                        </div>
                        <!--end::Col header-->
                        <!--begin::Card-->
                        <div class="d-questions-list">

                            <div class="card mb-6 mb-xl-9" v-for="(item, index) in pages_one" :key="index">
                                <!--begin::Card body-->
                                <div class="card-body">
                                    <!--begin::Header-->
                                    <div class="d-flex flex-stack mb-3">
                                        <!--begin::Badge-->
                                        <div class="badge badge-light">Question # {{index + 1}}</div>
                                        <!--end::Badge-->
                                        <!--begin::Menu-->
                                        <div>
                                            &nbsp;
                                        </div>
                                        <!--end::Menu-->
                                    </div>
                                    <!--end::Header-->
                                    <!--begin::Title-->
                                    <div class="mb-2">Q; {{item.question}}</div>
                                    <!--end::Title-->
                                    <!--begin::Content-->
                                    <div class="fs-6 fw-semibold text-gray-600 mb-5">A: {{item.answer}}</div>
                                    <!--end::Content-->
                                    <!--begin::Footer-->
                                    <div class="d-flex flex-stack flex-wrapr">
                                        <!--begin::Users-->
                                        <!--end::Users-->
                                        <!--begin::Stats-->
                                        <div class="d-flex my-1">
                                            <button class="btn btn-success" v-on:click="openEditQuestionForm(1, index)" data-bs-toggle="modal" data-bs-target="#add_question_modal">Edit</button>
                                            <button class="btn btn-danger" style="margin-left: 10px;">Remove</button>
                                        </div>
                                        <!--end::Stats-->
                                    </div>
                                    <!--end::Footer-->
                                </div>
                                <!--end::Card body-->
                            </div>
                        </div>
                        <!--end::Card-->
                        <button class="btn btn-primary er w-100 fs-6 px-8 py-4" data-bs-toggle="modal" v-on:click="assignPage(1)" data-bs-target="#add_question_modal">Create New Question for Page 1</button>
                    </div>
                    <!--end::Col--> 
                    <!--begin::Col-->
                    <div class="col-md-4 col-lg-12 col-xl-4">
                        <!--begin::Col header-->
                        <div class="mb-9">
                            <div class="d-flex flex-stack">
                                <div class="fw-bold fs-4">Page 2
                                <span class="fs-6 text-gray-400 ms-2">0</span></div>
                                <!--begin::Menu-->
                                <!--end::Menu-->
                            </div>
                            <div class="h-3px w-100 bg-primary"></div>
                        </div>
                        <div class="d-questions-list">

                            <div class="card mb-6 mb-xl-9" v-for="(item, index) in pages_two" :key="index">
                                <!--begin::Card body-->
                                <div class="card-body">
                                    <!--begin::Header-->
                                    <div class="d-flex flex-stack mb-3">
                                        <!--begin::Badge-->
                                        <div class="badge badge-light">Question # {{index + 1}}</div>
                                        <!--end::Badge-->
                                        <!--begin::Menu-->
                                        <div>
                                            &nbsp;
                                        </div>
                                        <!--end::Menu-->
                                    </div>
                                    <!--end::Header-->
                                    <!--begin::Title-->
                                    <div class="mb-2">Q; {{item.question}}</div>
                                    <!--end::Title-->
                                    <!--begin::Content-->
                                    <div class="fs-6 fw-semibold text-gray-600 mb-5">A: {{item.answer}}</div>
                                    <!--end::Content-->
                                    <!--begin::Footer-->
                                    <div class="d-flex flex-stack flex-wrapr">
                                        <!--begin::Users-->
                                        <!--end::Users-->
                                        <!--begin::Stats-->
                                        <div class="d-flex my-1">
                                            <button class="btn btn-success">Edit</button>
                                            <button class="btn btn-danger" style="margin-left: 10px;">Remove</button>
                                        </div>
                                        <!--end::Stats-->
                                    </div>
                                    <!--end::Footer-->
                                </div>
                                <!--end::Card body-->
                            </div>
                        </div>
                        <!--end::Col header-->
                        <button class="btn btn-primary er w-100 fs-6 px-8 py-4" data-bs-toggle="modal" v-on:click="assignPage(2)" data-bs-target="#add_question_modal">Create New Question for Page 2</button>
                    </div>
                    <!--end::Col-->
                    <!--begin::Col-->
                    <div class="col-md-4 col-lg-12 col-xl-4">
                        <!--begin::Col header-->
                        <div class="mb-9">
                            <div class="d-flex flex-stack">
                                <div class="fw-bold fs-4">Page 3 
                                <span class="fs-6 text-gray-400 ms-2">0</span></div>
                                <!--begin::Menu-->
                                <!--end::Menu-->
                            </div>
                            <div class="h-3px w-100 bg-success"></div>
                        </div>
                        <div class="d-questions-list">

                            <div class="card mb-6 mb-xl-9" v-for="(item, index) in pages_three" :key="index">
                                <!--begin::Card body-->
                                <div class="card-body">
                                    <!--begin::Header-->
                                    <div class="d-flex flex-stack mb-3">
                                        <!--begin::Badge-->
                                        <div class="badge badge-light">Question # {{index + 1}}</div>
                                        <!--end::Badge-->
                                        <!--begin::Menu-->
                                        <div>
                                            &nbsp;
                                        </div>
                                        <!--end::Menu-->
                                    </div>
                                    <!--end::Header-->
                                    <!--begin::Title-->
                                    <div class="mb-2">Q; {{item.question}}</div>
                                    <!--end::Title-->
                                    <!--begin::Content-->
                                    <div class="fs-6 fw-semibold text-gray-600 mb-5">A: {{item.answer}}</div>
                                    <!--end::Content-->
                                    <!--begin::Footer-->
                                    <div class="d-flex flex-stack flex-wrapr">
                                        <!--begin::Users-->
                                        <!--end::Users-->
                                        <!--begin::Stats-->
                                        <div class="d-flex my-1">
                                            <button class="btn btn-success">Edit</button>
                                            <button class="btn btn-danger" style="margin-left: 10px;">Remove</button>
                                        </div>
                                        <!--end::Stats-->
                                    </div>
                                    <!--end::Footer-->
                                </div>
                                <!--end::Card body-->
                            </div>
                        </div>
                        <!--end::Col header-->
                        <button class="btn btn-primary er w-100 fs-6 px-8 py-4" data-bs-toggle="modal" v-on:click="assignPage(3)" data-bs-target="#add_question_modal">Create New Question for Page 3</button>
                    </div>
                    <!--end::Col-->
                </div>
                <!--end::Row-->
                <div class="modal fade" tabindex="-1" id="add_question_modal">
                    <div class="modal-dialog modal-dialog-centered modal-dialog-scrollable">
                        <div class="modal-content">
                            <div class="modal-header">
                                <h5 class="modal-title">Question for page {{selectedPage}}</h5>

                                <!--begin::Close-->
                                <div class="btn btn-icon btn-sm btn-active-light-primary ms-2" data-bs-dismiss="modal" aria-label="Close">
                                    <span class="svg-icon svg-icon-2x">X</span>
                                </div>
                                <!--end::Close-->
                            </div>

                            <div class="modal-body">
                                <div class="d-add-question-modal">
                                    <div class="mb-10">
                                        <label for="exampleFormControlInput1" class="required form-label">Question</label>
                                        <input v-model="new_question.question" type="email" class="form-control form-control-solid" placeholder="Example input"/>
                                    </div>
                                    <div class="mb-10">
                                        <label for="exampleFormControlInput1" class="required form-label">Answer</label>
                                        <input v-model="new_question.answer" type="email" class="form-control form-control-solid" placeholder="Example input"/>
                                    </div>
                                </div>
                            </div>

                            <div class="modal-footer">
                                <button type="button" class="btn btn-light" data-bs-dismiss="modal">Close</button>
                                <button type="button" class="btn btn-primary" v-on:click="save_question">Save changes</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'addPrePay',
        data () {
            return {
                selectedPage: '',
                prepay_id: 0,
                new_question: {
                    question: '',
                    answer: ''
                },
                editedQuestion: '',
				pages_one: [
                    {
                        id: 1,
                        question: "sample question",
                        answer: "sample answer",
                    },
                    {
                        id: 2,
                        question: "sAnother ample question",
                        answer: "sample answer",
                    }
                ],
                pages_two: [
                ],
                pages_three: [
                ]
            }
        },
        methods: {
			assignPage(dPage){
                console.log('sellected page ->', dPage);
                this.selectedPage = dPage;
            },
            save_question(){
                console.log(this.new_question);//

                // build params
                $params = {
                    question: this.new_question.question,
                    answer: this.new_question.answer,
                    page: this.selectedPage
                };
            },
            hasPtoId(){
                console.log('has id -> ', this.$route.query);
                this.prepay_id = this.$route.query.id
            },
            openEditQuestionForm(page, refid){
                let reference_page = [];
                if(page == 1){
                    reference_page = this.pages_one;
                }

                if(page == 2){
                    reference_page = this.pages_two;
                }

                if(page == 3){
                    reference_page = this.pages_three;
                }

                console.log(reference_page[refid]);
                
            }
        },
        mounted: function(){
            this.hasPtoId();
        }
    }
</script>
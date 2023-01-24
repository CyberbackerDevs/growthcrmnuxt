<template>
    <!--begin::Timeline content-->
    <div class="timeline-content mb-10 mt-n1">
        <!--begin::Timeline heading-->
        <div class="pe-3 mb-5">
            <!--begin::Title-->
            <div class="fs-5 fw-semibold mb-2">Business Evaluation</div>
            <!--end::Title-->
            <!--begin::Description-->
            <div class="d-flex align-items-center mt-1 fs-6"><div class="text-muted me-2 fs-7">Added at 4:23 PM by Arphie Balboa</div></div>
            <!--end::Description-->
        </div>
        <!--end::Timeline heading-->

        <!--begin::Timeline details-->
        <div class="overflow-auto pb-5">
            
            <div class="alert alert-dismissible bg-light-warning border border-warning d-flex flex-column flex-sm-row w-100 p-5 mb-10">
                <div class="timeline-icon symbol symbol-circle symbol-50px me-4 mb-5 mb-sm-0">
                    <div class="symbol-label bg-warning">
                        <i class="bi bi-exclamation-diamond fs-2x text-white"></i>
                    </div>
                </div>
                <div class="d-flex flex-column pe-0 pe-sm-10">
                    <h5 class="mb-1">There is no Business Evaluation schedule booked for the client</h5>
                    <span>Please book a schedule in the nearest available schedule for the client</span>
                </div>

                <button type="button" class="position-absolute position-md-relative m-2 w-25 m-sm-0 top-0 end-0 btn btn-warning text-black ms-sm-auto">
                    Book a schedule
                </button>
            </div>

            <div class="alert alert-dismissible bg-light-info border border-info d-flex flex-column flex-sm-row w-100 p-5 mb-10">
                <div class="timeline-icon symbol symbol-circle symbol-50px me-4 mb-5 mb-sm-0">
                    <div class="symbol-label bg-info">
                        <i class="bi bi-headset fs-2x text-white"></i>
                    </div>
                </div>
                <div class="d-flex flex-column pe-0 pe-sm-10">
                    <h5 class="mb-1">January 31, 2023 has been booked by John Peter Doe for the client</h5>
                    <span>For any changes, please adjust to a new schedule</span>
                </div>
                <button type="button" class="position-absolute position-md-relative m-2 w-250px m-sm-0 top-0 end-0 btn btn-info text-white ms-sm-auto">
                    Reschedule Appointment
                </button>
                <button type="button" class="position-absolute position-md-relative m-2 w-250px m-sm-0 top-0 end-0 btn btn-warning text-black ms-sm-auto">
                    Follow Up Instance
                </button>
            </div>

            <div class="align-items-center border border-dashed border-gray-300 rounded min-w-700px p-7">
                <div class="d-schedule-header">
                    <h3 class="card-title align-items-start flex-column">
                        <span class="card-label fw-bold text-dark">Book a Schedule</span><br /><span class="text-muted mt-1 fw-semibold fs-7">Please provide a concise schedule for the client</span>
                    </h3>
                </div>
                <div class="d-flex flex-center flex-column">
                    <div class="d-schedule-body text-left w-75">
                        <div class="row d-month-part">
                            <div class="col-md-4">
                                <label for="exampleFormControlInput1" class="required form-label">Month</label>
                                <select class="form-select" aria-label="Select a Month">
                                    <option>Month</option>
                                    <option value="1">One</option>
                                    <option value="2">Two</option>
                                    <option value="3">Three</option>
                                </select>
                            </div>
                            <div class="col-md-4">
                                <label for="exampleFormControlInput1" class="required form-label">Day</label>
                                <select class="form-select" aria-label="Select a Day">
                                    <option>Date</option>
                                    <option value="1">One</option>
                                    <option value="2">Two</option>
                                    <option value="3">Three</option>
                                </select>
                            </div>
                            <div class="col-md-4">
                                <label for="exampleFormControlInput1" class="required form-label">Year</label>
                                <select class="form-select" aria-label="Select a Year">
                                    <option>Year</option>
                                    <option value="1">One</option>
                                    <option value="2">Two</option>
                                    <option value="3">Three</option>
                                </select>
                            </div>
                        </div>
                        <div class="row d-month-part">
                            <div class="col-md-4">
                                <label for="exampleFormControlInput1" class="required form-label">Hour</label>
                                <select class="form-select" aria-label="Select an Hour">
                                    <option>Month</option>
                                    <option value="1">One</option>
                                    <option value="2">Two</option>
                                    <option value="3">Three</option>
                                </select>
                            </div>
                            <div class="col-md-4">
                                <label for="exampleFormControlInput1" class="required form-label">Minute</label>
                                <select class="form-select" aria-label="Select a Minute">
                                    <option>Date</option>
                                    <option value="1">One</option>
                                    <option value="2">Two</option>
                                    <option value="3">Three</option>
                                </select>
                            </div>
                            <div class="col-md-4">
                                <label for="exampleFormControlInput1" class="required form-label">AM/PM</label>
                                <select class="form-select" aria-label="AM or PM">
                                    <option>Year</option>
                                    <option value="1">One</option>
                                    <option value="2">Two</option>
                                    <option value="3">Three</option>
                                </select>
                            </div>
                        </div>
                        <div class="d-flex flex-center flex-wrap" style="margin-top: 20px;">
                            <a href="#" class="btn btn-outline btn-outline-primary btn-active-primary m-2">Cancel</a>
                            <a href="#" class="btn btn-success m-2">Book now</a>
                        </div>
                    </div>
                </div>
            </div>

            <div class="align-items-center border border-dashed border-gray-300 rounded min-w-700px p-7">
                <div class="d-schedule-header">
                    <h3 class="card-title align-items-start flex-column">
                        <span class="card-label fw-bold text-dark">Add a follow up instance</span><br /><span class="text-muted mt-1 fw-semibold fs-7">Please provide a concise follow up instance from the client</span>
                    </h3>
                </div>
                <div class="d-flex flex-center flex-column">
                    <div class="d-schedule-body text-left w-75">
                        <div class="row d-month-part">
                            <div class="col-md-4">
                                <label for="exampleFormControlInput1" class="required form-label">Month</label>
                                <select class="form-select" aria-label="Select a Month">
                                    <option>Month</option>
                                    <option value="1">One</option>
                                    <option value="2">Two</option>
                                    <option value="3">Three</option>
                                </select>
                            </div>
                            <div class="col-md-4">
                                <label for="exampleFormControlInput1" class="required form-label">Day</label>
                                <select class="form-select" aria-label="Select a Day">
                                    <option>Date</option>
                                    <option value="1">One</option>
                                    <option value="2">Two</option>
                                    <option value="3">Three</option>
                                </select>
                            </div>
                            <div class="col-md-4">
                                <label for="exampleFormControlInput1" class="required form-label">Year</label>
                                <select class="form-select" aria-label="Select a Year">
                                    <option>Year</option>
                                    <option value="1">One</option>
                                    <option value="2">Two</option>
                                    <option value="3">Three</option>
                                </select>
                            </div>
                        </div>
                        <div class="row d-month-part">
                            <div class="col-md-4">
                                <label for="exampleFormControlInput1" class="required form-label">Hour</label>
                                <select class="form-select" aria-label="Select an Hour">
                                    <option>Month</option>
                                    <option value="1">One</option>
                                    <option value="2">Two</option>
                                    <option value="3">Three</option>
                                </select>
                            </div>
                            <div class="col-md-4">
                                <label for="exampleFormControlInput1" class="required form-label">Minute</label>
                                <select class="form-select" aria-label="Select a Minute">
                                    <option>Date</option>
                                    <option value="1">One</option>
                                    <option value="2">Two</option>
                                    <option value="3">Three</option>
                                </select>
                            </div>
                            <div class="col-md-4">
                                <label for="exampleFormControlInput1" class="required form-label">AM/PM</label>
                                <select class="form-select" aria-label="AM or PM">
                                    <option>Year</option>
                                    <option value="1">One</option>
                                    <option value="2">Two</option>
                                    <option value="3">Three</option>
                                </select>
                            </div>
                        </div>
                        <div class="d-flex flex-center flex-wrap" style="margin-top: 20px;">
                            <a href="#" class="btn btn-outline btn-outline-primary btn-active-primary m-2">Cancel</a>
                            <a href="#" class="btn btn-success m-2">Book now</a>
                        </div>
                    </div>
                </div>
            </div>

            

        </div>
        <!--end::Timeline details-->
    </div>
    <!--end::Timeline content-->    
</template>
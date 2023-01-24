<template>
    <div class="d-add-new-attendance">
        <div class="d-add-attendance" v-on:click="addCbAttendance">Add new attendance <span class="d-plus-icon">+</span></div>
        <v-dialog v-model="openAddAttendance" width="700">
            <v-card>
                <!-- <v-card-title class="text-h5 grey lighten-2">&nbsp;</v-card-title> -->

                <v-card-text style="padding: 15px;">
                    <div class="d-new-attendance">
                        <div class="d-new-attendance-inner">
                            <div class="d-new-at-date">
                                <v-date-picker dark v-model="newATDate"></v-date-picker>
                            </div>
                        </div>
                        <div class="d-new-timed">
                            <div class="d-new-timed-inner">
                                <div class="d-nt-tiel">Login Time</div>
                                <div class="d-new-timed-login d-tp-formater">
                                    <div class="d-nt-hour">
                                        <input type="number" placeholder="00"/>
                                    </div>
                                    <div class="d-nt-sep">:</div>
                                    <div class="d-nt-minute">
                                        <input type="number" placeholder="00"/>
                                    </div>
                                    <div class="d-time-range">
                                        <button v-on:click="selectRangeOpt('login', 'am')">am</button>
                                        <button v-on:click="selectRangeOpt('login', 'pm')">pm</button>
                                    </div>
                                </div>
                                <div class="d-nt-tiel">Logout Time</div>
                                <div class="d-new-timed-logout d-tp-formater">
                                    <div class="d-nt-hour">
                                        <input type="number" placeholder="00"/>
                                    </div>
                                    <div class="d-nt-sep">:</div>
                                    <div class="d-nt-minute">
                                        <input type="number" placeholder="00"/>
                                    </div>
                                    <div class="d-time-range">
                                        <button v-on:click="selectRangeOpt('logout', 'am')">am</button>
                                        <button v-on:click="selectRangeOpt('logout', 'pm')">pm</button>
                                    </div>
                                </div>
                                <div class="d-nt-tiel">Reason</div>
                                <div class="d-nt-reason-for-injection">
                                    <textarea name="" id=""></textarea>
                                </div>
                                <div class="opt-add-at">
                                    <button>Cancel</button>
                                    <button>Save</button>
                                </div>
                            </div>
                        </div>
                    </div>
                </v-card-text>
                    <!-- <v-divider></v-divider>

                        <v-card-actions>
                            <v-spacer></v-spacer>
                            save
                            
                        </v-card-actions> -->
            </v-card>
        </v-dialog>
    </div>
</template>

<script>
    export default {
        name: 'AttendanceComponent',
        data () {
            return {
                newATDate: (new Date(Date.now() - (new Date()).getTimezoneOffset() * 60000)).toISOString().substr(0, 10),
                openAddAttendance: false,
            }
        },
        methods: {
            addCbAttendance(){
                this.openAddAttendance = true;
            },
            loadInitialValues(){

            }
        },
        mounted(){
            this.loadInitialValues();
        }
    }
</script>

<style scoped>
    input[type='number'] {
        -moz-appearance:textfield;
    }

    input::-webkit-outer-spin-button,
    input::-webkit-inner-spin-button {
        -webkit-appearance: none;
    }
    .d-add-attendance {
        background: #4a4a4a;
        color: #fff;
        text-align: center;
        margin: 0 1% 10px;
        text-transform: uppercase;
        font-weight: 700;
        padding: 15px 0;
        border-radius: 5px;
        letter-spacing: 2px;
        cursor: pointer;
    }
    .d-new-attendance-inner {
        display: inline-block;
        width: 50%;
        vertical-align: middle;
    }
    .d-new-timed {
        display: inline-block;
        width: 48%;
        vertical-align: middle;
    }
    .d-tp-formater > div {
        display: inline-block;
        vertical-align: middle;
    }
    .d-tp-formater input {
        border-bottom: 2px solid #333;
        width: 100%;
        padding: 7px 10px;
        line-height: 1em;
        /* border-radius: 10px; */
        font-size: 21px;
        font-weight: bold;
    }
    .d-tp-formater .d-nt-hour{
        width: 15%;
    }
    .d-tp-formater .d-nt-sep{
        width: 5%;
        text-align: center;
        font-weight: bold;
        font-size: 30px;
        line-height: 1em;
        color: #333;
    }
    .d-tp-formater .d-nt-minute{
        width: 15%;
    }

    .d-tp-formater .d-time-range {
        margin-left: 15px;
    }

    .d-tp-formater .d-time-range button {
        display: inline-block;
        vertical-align: middle;
        color: #333;
        font-size: 14px;
        border: 2px solid #333;
        line-height: 1em;
        padding: 8px;
        border-radius: 100px;
        font-weight: bold;
        text-transform: uppercase;
    }

    .d-nt-reason-for-injection textarea {
        border-bottom: 2px solid #333;
        width: 100%;
        padding: 7px 10px;
        line-height: 1em;
        /* border-radius: 10px; */
        font-size: 21px;
        min-height: 90px;
    }
    .d-nt-tiel {
        font-size: 18px;
        font-weight: 700;
        margin-bottom: 0px;
    }
    .opt-add-at {
        margin-top: 15px;
        text-align: right;
    }

    .opt-add-at button {
        background: #333;
        color: #fff;
        line-height: 1em;
        text-transform: uppercase;
        padding: 10px 15px;
        border-radius: 100px;
    }
    
</style>
<template>
    <div class="d-profile-attendance">
        <div class="d-section-header">
            <span>Cyberbacker Attendance</span>
            <hr />
        </div>
        <div class="d-profile-attendance-inner">
            <div class="d-profile-attendance-list">
                <ProfileAddAttendance />
                <div class="d-profile-at-item" v-for="(item, index) in attendanceInfo" :key="index">
                    <div class="d-profile-itm-day">{{item.date_day}} | {{item.date_month}} {{item.date_date}}, {{item.date_year}}</div>
                    <div class="d-profile-itm-info">
                        <div class="d-profile-status">{{item.status}}</div>
                        <div class="d-profile-date"> from {{item.login}} to {{item.logout}}</div>
                    </div>
                    <div class="d-profile-time-spent">
                        08:38
                    </div>
                    <div class="d-profile-itm-activity">
                        <button v-on:click="openDisputeInfo(item)">Adjust</button>
                    </div>
                    
                </div>
            </div>
            
        </div>
        <div class="modal-info-section">
            <v-dialog v-model="openDisputeModal" width="500">
                <v-card>
                    <v-card-title class="text-h5 grey lighten-2">Adjust Attendance for {{selectedAttendanceItem.date_month}} {{selectedAttendanceItem.date_date}} of {{selectedAttendanceItem.date_year}}</v-card-title>

                    <v-card-text>
                        <div class="d-despute-form">
                            <div class="dd-form-info">
                                <div class="dd-form-into">
                                    <div class="dd-form-status">Status: {{selectedAttendanceItem.status}}</div>
                                    <div class="dd-form-status">Login: {{selectedAttendanceItem.login}}</div>
                                    <div class="dd-form-status">Logout: {{selectedAttendanceItem.logout}}</div>
                                </div>
                            </div>
                            <div class="d-option-infos">
                                <div class="dd-form-item">
                                    <div class="dd-form-label">Adjust login time</div>
                                    <div class="dd-form-numbers">
                                        <div class="dd-form-time">
                                            <div class="dd-form-hour-inner">
                                                <v-select
                                                    v-model="selectedLoginHour"
                                                    :items="defaultLoginHour"
                                                    label="Hour"
                                                ></v-select>
                                            </div>
                                            <div class="dd-form-minutes-inner">
                                                <v-select
                                                    v-model="selectedLoginMinute"
                                                    :items="defaultLoginMinute"
                                                    label="Minute"
                                                ></v-select>
                                            </div>
                                            <div class="dd-form-lm-inner">
                                                <v-select
                                                    v-model="selectedLoginTime"
                                                    :items="defaultLoginDayTime"
                                                    label="am/pm"
                                                ></v-select>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="dd-form-item">
                                    <div class="dd-form-label">Adjust logout time</div>
                                    <div class="dd-form-numbers">
                                        <div class="dd-form-time">
                                            <div class="dd-form-hour-inner">
                                                <v-select
                                                    v-model="selectedLogoutHour"
                                                    :items="defaultLogoutHour"
                                                    label="Hour"
                                                ></v-select>
                                            </div>
                                            <div class="dd-form-minutes-inner">
                                                <v-select
                                                    v-model="selectedLogoutMinute"
                                                    :items="defaultLogoutMinute"
                                                    label="Minute"
                                                ></v-select>
                                            </div>
                                            <div class="dd-form-lm-inner">
                                                <v-select
                                                    v-model="selectedLogoutTime"
                                                    :items="defaultLogoutDayTime"
                                                    label="am/pm"
                                                ></v-select>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </v-card-text>

                    <v-divider></v-divider>

                    <v-card-actions>
                        <v-spacer></v-spacer>
                        <div class="initial_save_info" v-if="showInitials">
                            <v-btn color="primary" text v-on:click="closeAdjustment" >Cancel</v-btn>
                            <v-btn color="primary" text v-on:click="initialSaveAdjustment" >Save Adjustment</v-btn>
                        </div>
                        <div class="final_save_info" v-if="showFinalConfirmation">
                            <v-btn color="primary" text v-on:click="cancelConfirmation" >Cancel</v-btn>
                            <v-btn color="primary" text v-on:click="confirmAdjustment" >Confirm</v-btn>
                        </div>
                        
                    </v-card-actions>
                </v-card>
            </v-dialog>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'AttendanceComponent',
        data () {
            return {
                showInitials: true,
                showFinalConfirmation: false,
                time: '',
                menu2: false,
                openDisputeModal: false,
                openAddAttendance: false,
                selectedAttendanceItem: {},
                defaultLoginHour: [],
                defaultLoginMinute: [],
                defaultLogoutHour: [],
                defaultLogoutMinute: [],
                defaultLoginDayTime: ['AM', 'PM'],
                defaultLogoutDayTime: ['AM', 'PM'],
                selectedLoginHour: '',
                selectedLoginMinute: '',
                selectedLoginTime: '',
                selectedLogoutHour: '',
                selectedLogoutMinute: '',
                selectedLogoutTime: '',
                attendanceInfo: [
                    {
                        date_day: "Sunday",
                        date_month: "Nov",
                        date_date: "21",
                        date_year: "2022",
                        status: "Present",
                        login: "8:45 AM",
                        logout: "5:45 PM",
                    },
                    {
                        date_day: "Monday",
                        date_month: "Nov",
                        date_date: "21",
                        date_year: "2022",
                        status: "Present",
                        login: "8:45 AM",
                        logout: "5:45 PM",
                    },
                    {
                        date_day: "Monday",
                        date_month: "Nov",
                        date_date: "21",
                        date_year: "2022",
                        status: "Present",
                        login: "8:45 AM",
                        logout: "5:45 PM",
                    },
                    {
                        date_day: "Monday",
                        date_month: "Nov",
                        date_date: "21",
                        date_year: "2022",
                        status: "Present",
                        login: "8:45 AM",
                        logout: "5:45 PM",
                    },
                    {
                        date_day: "Monday",
                        date_month: "Nov",
                        date_date: "21",
                        date_year: "2022",
                        status: "Present",
                        login: "8:45 AM",
                        logout: "5:45 PM",
                    },
                    {
                        date_day: "Monday",
                        date_month: "Nov",
                        date_date: "21",
                        date_year: "2022",
                        status: "Present",
                        login: "8:45 AM",
                        logout: "5:45 PM",
                    },
                    {
                        date_day: "Monday",
                        date_month: "Nov",
                        date_date: "21",
                        date_year: "2022",
                        status: "Present",
                        login: "8:45 AM",
                        logout: "5:45 PM",
                    },
                    {
                        date_day: "Monday",
                        date_month: "Nov",
                        date_date: "21",
                        date_year: "2022",
                        status: "Present",
                        login: "8:45 AM",
                        logout: "5:45 PM",
                    },
                    {
                        date_day: "Monday",
                        date_month: "Nov",
                        date_date: "21",
                        date_year: "2022",
                        status: "Present",
                        login: "8:45 AM",
                        logout: "5:45 PM",
                    },
                    {
                        date_day: "Monday",
                        date_month: "Nov",
                        date_date: "21",
                        date_year: "2022",
                        status: "Present",
                        login: "8:45 AM",
                        logout: "5:45 PM",
                    },
                ]
            }
        },
        methods: {
            closeAdjustment(){
                this.openDisputeModal = false;
            },
            cancelConfirmation(){
                this.showInitials = true;
                this.showFinalConfirmation = false;
            },
            openDisputeInfo(attendanceForm){
                console.log('attendance id -> ', attendanceForm);
                // disect login
                let login_info = attendanceForm.login.split(' ');
                this.selectedLoginTime = login_info[1]; // assign AM and PM
                let loginTimeInfo = login_info[0].split(":");
                this.selectedLoginHour = parseInt(loginTimeInfo[0]);
                this.selectedLoginMinute = parseInt(loginTimeInfo[1]);

                // disect logout
                let logout_info = attendanceForm.logout.split(' ');
                this.selectedLogoutTime = logout_info[1]; // assign AM and PM
                let logoutTimeInfo = logout_info[0].split(":");
                this.selectedLogoutHour = parseInt(logoutTimeInfo[0]);
                this.selectedLogoutMinute = parseInt(logoutTimeInfo[1]);

                this.openDisputeModal = true;
                this.selectedAttendanceItem = attendanceForm;
            },
            initialSaveAdjustment(){
                this.showInitials = false;
                this.showFinalConfirmation = true;
            },
            confirmAdjustment(){
                console.log('update the item');
            },
            addCbAttendance(){
                console.log('open new form');
                
            },
            loadDefaultFormValues(){
                for (let index = 1; index <= 12; index++) {
                    this.defaultLoginHour.push(index);
                    this.defaultLogoutHour.push(index);
                }

                for (let index = 1; index <= 60; index++) {
                    this.defaultLoginMinute.push(index);
                    this.defaultLogoutMinute.push(index);
                }
            }
        },
        mounted(){
            this.loadDefaultFormValues();
        }
    }
</script>

<style scoped>
    .d-profile-at-item {
        width: 98%;
        margin: 0 auto 10px;
        border: 1px solid #4a4a4a;
        border-radius: 5px;
    }
    .d-profile-at-item > div {
        display: inline-block;
        vertical-align: middle;
    }
    .d-profile-at-item .d-profile-itm-day {
        width: 20%;
        font-size: 15px;
        font-weight: 700;
        padding: 15px 20px;
        background: #4a4a4a;
        color: #fff;
        text-transform: uppercase;
    }
    .d-profile-at-item .d-profile-time-spent {
        width: 20%;
        padding-left: 20px;
        font-size: 30px;
        font-weight: bold;
        /* font-family: 'Covered By Your Grace', cursive; */
        line-height: 1em;
        text-align: center;
        color: #4a4a4a;
    }
    .d-profile-at-item .d-profile-itm-info {
        width: 30%;
        padding-left: 20px;
    }
    .d-profile-at-item .d-profile-itm-activity {
        width: 24%;
        text-align: right;
    }
    .d-profile-at-item .d-profile-itm-info .d-profile-status {
        font-weight: 700;
        font-size: 19px;
        line-height: 1em;
    }
    .d-profile-at-item .d-profile-itm-info .d-profile-date {
        font-size: 14px;
        color: #939393;
    }
    .d-profile-itm-activity button {
        background: #4a4a4a;
        color: #fff;
        font-size: 14px;
        font-weight: 400;
        line-height: 1em;
        padding: 8px 15px;
        border-radius: 25px;
        text-transform: uppercase;
    }

    .d-option-infos > .dd-form-item {
        display: inline-block;
        width: 45%;
        margin: 0 2%;
    }
    .d-option-infos {
        margin-top: 20px;
    }
    .dd-form-item .dd-form-label {
        /* font-family: 'Covered By Your Grace', cursive; */
        font-size: 22px;
        text-align: center;
        font-weight: bold;
        margin-bottom: 15px;
    }
    .dd-form-time .dd-form-hour-inner,
    .dd-form-time .dd-form-minutes-inner,
    .dd-form-time .dd-form-lm-inner {
        display: inline-block;
        width: 28%;
        margin: 0 2%;
    }
    
    
</style>
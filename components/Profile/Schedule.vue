<template>
    <div class="d-schedule-info">
        <div class="d-section-header">
            <span>Active Schedule</span>
            <hr />
        </div>
        <div class="d-schedule-table">
            <div class="d-schedule-item" v-for="(item, index) in schedule" :key="index">
                <div class="d-schedule-day">{{item.name}}</div>
                <div class="d-schedule-time">{{item.time}}</div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'AttendanceComponent',
        data () {
            return {
                schedule: [
                    {
                        name: "Sunday",
                        time: "7:00am-5:00pm"
                    },
                    {
                        name: "Monday",
                        time: "7:00am-5:00pm"
                    },
                    {
                        name: "Tuesday",
                        time: "7:00am-5:00pm"
                    },
                    {
                        name: "Wednesday",
                        time: "7:00am-5:00pm"
                    },
                    {
                        name: "Thursday",
                        time: "7:00am-5:00pm"
                    },
                    {
                        name: "Friday",
                        time: "7:00am-5:00pm"
                    },
                    {
                        name: "Saturday",
                        time: "7:00am-5:00pm"
                    },
                ]
            }
        }
    }
</script>

<style scoped>
    .d-schedule-table {
        text-align: center;
        margin-bottom: 15px;
    }
    .d-schedule-table .d-schedule-item {
        display: inline-block;
        width: 13%;
        margin: 0 .5%;
        border: 1px solid #4a4a4a;
        border-radius: 5px;
    }
    .d-schedule-table .d-schedule-item .d-schedule-day {
        background: #4a4a4a;
        color: #fff;
        text-transform: uppercase;
        font-size: 14px;
        padding: 7px 0;
    }
    .d-schedule-table .d-schedule-item .d-schedule-time {
        padding: 10px 0;
        font-size: 15px;
    }
    .d-schedule-info {
        margin-bottom: 60px;
    }
</style>
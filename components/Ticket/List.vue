<template>
    <div class="d-ticket-list">
        <div class="d-list-title">Unassigned Tickets</div>
        <div class="d-ticket-items">
            <div class="d-ticket-header">
                <div class="d-ticket-sender">Created By</div>
                <div class="d-ticket-subject">Subject</div>
                <div class="d-ticket-assigned">Assigned</div>
                <div class="d-ticket-status">Status</div>
                <div class="d-ticket-privacy">Priority</div>
                <div class="d-ticket-created">Created At</div>
            </div>
            <div class="d-ticket-item" v-for="n in 10">
                <div class="d-ticket-item-inner">
                    <div class="d-ticket-sender">
                        <div class="d-ticket-icon">
                            <div class="d-ticket-circle">SM</div>
                        </div>
                        <div class="d-ticket-details">
                            <div class="d-ticket-name">Samuel Manuel</div>
                            <div class="d-ticket-position">Cyberbacker</div>
                        </div>
                    </div>
                    <div class="d-ticket-subject">
                        <div class="d-ticket-subject">Issues with AT</div>
                        <div class="d-ticket-subject-id">#23124</div>
                    </div>
                    <div class="d-ticket-assigned">
                        <div class="d-ticket-assigned">none</div>
                    </div>
                    <div class="d-ticket-status">
                        <div class="d-status-base tck-active">Fresh</div>
                    </div>
                    <div class="d-ticket-privacy">
                        <div class="d-prio-base priority">Normal</div>
                    </div>
                    <div class="d-ticket-created">
                        <div class="dmillk-lactose">Nov. 21. 20222</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'CTicketList',
        data () {
            return {
                dialog: false,
                toShow: 'list'
            }
        },
        methods: {
            openSpecificPayslip(){
                this.dialog = true;
            }
        }
    }
</script>

<style scoped>
    .d-ticket-header > div,
    .d-ticket-item-inner > div {
        display: inline-block;
        vertical-align: middle;
    }

    .d-ticket-header > .d-ticket-sender,
    .d-ticket-item-inner > .d-ticket-sender {
        width: 20%;
    }

    .d-ticket-item-inner > .d-ticket-sender .d-ticket-icon {
        display: inline-block;
        width: 30%;
        vertical-align: middle;
    }
    .d-ticket-item-inner > .d-ticket-sender .d-ticket-icon .d-ticket-circle {
        background: #333;
        text-align: center;
        color: #fff;
        width: 60px;
        height: 60px;
        padding: 10px;
        border-radius: 60px;
        font-size: 33px;
        font-family: 'Covered By Your Grace', cursive;
        font-weight: bold;
    }
    .d-ticket-item-inner > .d-ticket-sender .d-ticket-details {
        display: inline-block;
        width: 68%;
        vertical-align: middle;
    }

    .d-ticket-header > .d-ticket-subject,
    .d-ticket-item-inner > .d-ticket-subject {
        width: 20%;
    }

    .d-ticket-header > .d-ticket-assigned,
    .d-ticket-item-inner > .d-ticket-assigned {
        width: 20%;
    }

    .d-ticket-header > .d-ticket-status,
    .d-ticket-item-inner > .d-ticket-status {
        width: 10%;
    }

    .d-ticket-header > .d-ticket-privacy,
    .d-ticket-item-inner > .d-ticket-privacy {
        width: 10%;
    }

    .d-ticket-header > .d-ticket-created,
    .d-ticket-item-inner > .d-ticket-created {
        width: 15%;
    }

    .d-ticket-item-inner {
        margin-bottom: 10px;
        padding: 0 20px 10px;
        border-bottom: 1px solid #e7e7e7;
    }

    .d-ticket-header {
        margin-bottom: 25px;
        font-size: 18px;
        font-weight: bold;
        padding: 0 20px;
    }

    .d-list-title {
        font-size: 24px;
        font-weight: 100;
        margin-bottom: 35px;
    }

    .d-ticket-position {
        font-size: 14px;
        color: #838383;
        margin-top: 3px;
    }

    .d-ticket-subject-id {
        font-size: 14px;
        color: #838383;
        margin-top: 3px;
    }
</style>
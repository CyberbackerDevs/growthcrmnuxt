<template>
    <div class="d-cb-profile">
        <div class="d-dashboard-inner">
            <div class="d-sidebar-main">
                menu here
            </div>
            <div class="d-main-content">
                <div class="d-main-content-inner">
                    <div class="d-ticket-side">
                        <div class="d-ts-inner">
                            <button>Sorting Table</button>
                            <button>Assigned to me</button>
                        </div>
                    </div>
                    <div class="d-ticket-main">
                        <div class="d-ticket-main-inner">
                            <div class="d-ticket-info" v-if="toShow == 'info'"><TicketInfo /></div>
                            <div class="d-ticket-list" v-if="toShow == 'list'"><TicketList /></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'CPayslip',
        data () {
            return {
                dialog: false,
                toShow: 'info'
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
    .d-main-content {
        background: #fff;
        padding: 10px;
        border-radius: 5px;
        box-shadow: 0 0 12px #efefef;
    }

    .d-ticket-side {
        display: inline-block;
        width: 20%;
        vertical-align: top;
    }

    .d-ticket-main {
        display: inline-block;
        width: 78%;
        vertical-align: middle;
    }

    .d-main-content-inner {
        margin-top: 25px;
    }

    .d-ts-inner button {
        display: block;
        width: 100%;
        background: #919191;
        text-align: left;
        color: #fff;
        margin-bottom: 10px;
        border-radius: 5px;
        line-height: 1em;
        padding: 10px 15px;
    }

    .d-ts-inner button:hover {
        background: #919191;
    }

    .d-ts-inner {
        margin-left: 30px;
        margin-right: 20px;
    }

    .d-main-content-inner {
        margin-top: 25px;
    }
</style>
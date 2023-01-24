<template>
    <div class="d-cb-profile">
        <div class="d-dashboard-inner">
            <div class="d-sidebar-main">
                menu here
            </div>
            <div class="d-main-content">
                <div class="d-main-content-inner">
                    <div class="d-content-list">
                        <div class="d-profile-filter">filter</div>
                        <div class="d-search-form">
                            <div class="d-search-inner">
                                <input type="text" name="" id="" placeholder="Enter keyword">
                                <button>Search</button>
                            </div>
                        </div>
                        <div class="d-content-cb-list">
                            <div class="d-cblist-item" v-for="n in 10" v-on:click="openProfileItem()">
                                <div class="d-cb-image">
                                    <div class="d-cb-circle">SM</div>
                                </div>
                                <div class="d-cb-profile-details">
                                    <div class="d-cb-name">John peter doe</div>
                                    <div class="d-cb-last-login">Last login: November 24, 2022 18:42 MST</div>
                                </div>
                                <div class="d-cb-option">
                                    <button>&rsaquo;</button>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="d-content-stats">
                        <div class="d-has-profile-selcted" v-if="hasProfileSelected">
                            <div class="d-profile-inner">
                                <h2>John Peter Doe</h2>
                                <div class="d-profile-email">smaple@cyberbacker.com</div>
                                <div class="d-profile-options">
                                    <button>More Details</button>
                                    <button>Full Payrols</button>
                                </div>
                                <div class="profile-stats-main">
                                    <div class="profile-stat-item">
                                        <div class="stats-value">03</div>
                                        <div class="stats-label">Absents</div>
                                    </div>
                                    <div class="profile-stat-item">
                                        <div class="stats-value">06</div>
                                        <div class="stats-label">Late</div>
                                    </div>
                                    <div class="profile-stat-item">
                                        <div class="stats-value">00</div>
                                        <div class="stats-label">PTO</div>
                                    </div>
                                    <div class="profile-stat-item">
                                        <div class="stats-value">YES</div>
                                        <div class="stats-label">PrePay Form</div>
                                    </div>
                                </div>
                                <div class="d-page-title">Cyberbacker Running Payrol</div>
                                <div class="d-show-payslip">
                                    <div class="running-payslip-inner">
                                        <div class="d-separation-title">Inclusion</div>
                                        <div class="d-running-pay-item">
                                            <div class="dr-label">SF for Nov. 01 - Nov. 15</div>
                                            <div class="dr-valuet">27.27</div>
                                            <div class="dr-by">x</div>
                                            <div class="dr-quantity">8</div>
                                            <div class="dr-total">$218.18</div>
                                        </div>
                                        <div class="d-separation-title">Deduction</div>
                                        <div class="d-running-pay-item">
                                            <div class="dr-label">Absense for Nov. 01 - Nov. 1</div>
                                            <div class="dr-valuet">27.27</div>
                                            <div class="dr-by">x</div>
                                            <div class="dr-quantity">3</div>
                                            <div class="dr-total">$81.81</div>
                                        </div>
                                        <div class="d-running-pay-item">
                                            <div class="dr-label">CB Merch (jacket)</div>
                                            <div class="dr-valuet">35</div>
                                            <div class="dr-by">x</div>
                                            <div class="dr-quantity">1</div>
                                            <div class="dr-total">$35</div>
                                        </div>
                                        <div class="d-running-pay-item">
                                            <div class="dr-label">HMO (50%)</div>
                                            <div class="dr-valuet">20</div>
                                            <div class="dr-by">x</div>
                                            <div class="dr-quantity">1</div>
                                            <div class="dr-total">20</div>
                                        </div>
                                        <div class="d-running-pay-item">
                                            <div class="dr-label">Add Item</div>
                                            <div class="dr-valuet">20</div>
                                            <div class="dr-by">x</div>
                                            <div class="dr-quantity">1</div>
                                            <div class="dr-total">20</div>
                                        </div>
                                        <div class="d-running-total-item">
                                            <div class="dr-label">Total</div>
                                            <div class="dr-valuet">&nbsp;</div>
                                            <div class="dr-by">&nbsp;</div>
                                            <div class="dr-quantity">&nbsp;</div>
                                            <div class="dr-total">20</div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="no-selected" v-if="!hasProfileSelected">
                            <img src="@/assets/images/default_user_w.png"/>
                            <div class="d-profile-select">Please select a profile</div>
                        </div>
                    </div>
                    
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'indexProfile',
        data () {
            return {
                hasProfileSelected: false,
                cblist: [
                    {
                        name: 'test 1',
                        login: 13,
                        late: 2,
                        absent: 2,
                        pto: 2
                    }
                ]
            }
        },
        methods: {
            openProfileItem(){
                this.hasProfileSelected = true;
            }
        },
        mounted(){
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
    .cb-profile-info {
        vertical-align: top;
        display: inline-block;
        width: 25%;
        text-align: center;
    }

    .cb-profile-activity {
        vertical-align: top;
        display: inline-block;
        width: 73%;

    }

    .d-content-stats {
        display: inline-block;
        vertical-align: top;
        width: 64%;
    }

    .d-content-list {
        display: inline-block;
        vertical-align: top;
        width: 35%;
    }

    .d-cblist-item > div {
        display: inline-block;
        vertical-align: middle;
    }

    .d-cb-image {
        width: 15%;
    }

    .d-cb-circle {
        width: 60px;
        background: #ff8d00;
        color: #fff;
        font-family: 'Covered By Your Grace', cursive;
        text-align: center;
        padding: 12px;
        height: 60px;
        border-radius: 50px;
        font-size: 30px;
    }

    .d-cb-profile-details {
        width: 65%;
    }
    .d-cb-option {
        width: 15%;
        text-align: right;
    }

    .d-cblist-item {
        margin-bottom: 10px;
        padding: 0 15px 10px;
        border-bottom: 1px solid #ccc;
    }

    .d-stats-inner {
        text-align: left;
        padding-left: 45px;
    }

    .d-stats-item {
        display: inline-block;
        width: 47%;
        margin: 1% 1% 1%;
        background: #ccc;
        padding: 15px;
        border-radius: 3px;
        text-align: left;
    }

    .d-stats-title {
        font-size: 18px;
    }

    .d-icon {
        display: inline-block;
        width: 15%;
        vertical-align: middle;
    }

    .d-info {
        display: inline-block;
        width: 65%;
        vertical-align: middle;
    }

    .d-stats-link {
        display: inline-block;
        width: 15%;
        vertical-align: middle;
    }

    .d-stats-link button {
        background: #747474;
        color: #fff;
        height: 40px;
        width: 40px;
        border-radius: 100px;
        font-size: 26px;
        line-height: 1em;
        font-weight: 100;
        padding: 0px;
    }

    .d-stats-number {
        font-size: 24px;
        font-weight: 400;
    }
    .d-cb-option button {
        font-size: 45px;
        color: #ff8d00;
    }
    .progress-report {
        padding-left: 40px;
    }

    .no-selected {
        text-align: center;
        margin-top: 40px;
    }
    .no-selected img {
        width: 390px;
        background: #ff8d00;
        border-radius: 205px;
        box-shadow: 0 0 12px #ff8d00;
        border: 1px solid #ff8d00;
    }
    .d-profile-inner {
        padding-left: 40px;
        margin-top: 30px;
    }

    .profile-stats-main .profile-stat-item {
        display: inline-block;
        width: 24%;
        text-align: center;
    }

    .profile-stats-main {
        margin-top: 25px;
        border-top: 1px solid #ccc;
        border-bottom: 1px solid #ccc;
        padding: 10px 0;
    }

    .profile-stat-item .stats-label {
        text-transform: uppercase;
        font-weight: bold;
        font-size: 16px;
    }
    .profile-stat-item .stats-value {
        font-size: 40px;
        font-weight: 100;
    }

    .d-running-pay-item {
        border-bottom: 1px solid #ccc;
        padding: 10px 20px;
    }

    .d-running-total-item {
        border-bottom: 1px solid #ccc;
        padding: 10px 20px;
        background: #e7e7e7;
    }

    .d-running-pay-item > div {
        display: inline-block;
    }

    .d-running-total-item > div {
        display: inline-block;
    }


    .dr-label {
        width: 72%;
    }

    .dr-valuet {
        width: 8%;
        text-align: center;
    }

    .dr-by {
        width: 3%;
        text-align: center;
    }

    .dr-quantity {
        width: 3%;
        text-align: center;
    }

    .dr-total {
        width: 10%;
        text-align: right;
    }

    .d-page-title {
        margin-top: 30px;
        font-size: 22px;
        font-weight: 100;
        margin-bottom: 10px;
        border-bottom: 5px;
    }

    .d-separation-title {
        font-size: 19px;
        margin: 15px 0;
        font-weight: 100;
        font-style: italic;
    }

    .d-profile-options {
        margin: 20px;
    }

    .d-profile-options button {
        width: 47%;
        margin: 0 1%;
        background: #ff8d00;
        color: #fff;
        font-size: 20px;
        text-transform: uppercase;
        font-weight: 100;
        padding: 15px 0;
        border-radius: 5px;
        letter-spacing: 2px;
    }

    .running-payslip-inner {
        padding: 20px 20px;
        box-shadow: 0 0 12px #ccc;
        border-radius: 5px;
    }

    .d-search-form {
        margin-bottom: 25px;
    }
    .d-search-form .d-search-inner {
        text-align: center;
    }

    .d-search-form .d-search-inner input {
        display: block;
        width: 100%;
        border: 1px solid #ccc;
        font-size: 16px;
        padding: 10px 15px;
        border-radius: 5px;
        margin-bottom: 5px;
    }

    .d-search-form .d-search-inner button {
        background: #ff8d00;
        width: 100%;
        display: block;
        text-transform: uppercase;
        font-size: 16px;
        font-weight: 700;
        padding: 10px;
        border-radius: 5px;
        color: #fff;
    }

    .d-profile-select {
        font-family: 'Covered By Your Grace', cursive;
        font-size: 46px;
        margin-top: 15px;
    }
</style>
<template>
    <div class="d-cb-profile">
        <div class="d-dashboard-inner">
            <div class="d-sidebar-main">
                menu here
            </div>
            <div class="d-main-content">
                <div class="d-main-content-inner">
                    <div class="cb-profile-info">
                        <ProfileSideMenu />
                    </div>
                    <div class="cb-profile-activity">
                        <div class="cb-profile-activity-inner">
                            payslip here
                            

                            <v-dialog v-model="dialog" width="900">
                                <v-card>
                                    <v-card-title class="text-h5 grey lighten-2">
                                        November 1, 2022 to November 15, 2022
                                    </v-card-title>

                                    <v-card-text>
                                        <div class="d-payslip">
                                            <div class="d-header-part">
                                                <div class="d-logo-here"><img src="@/assets/images/logo_black.png"/></div>
                                                <div class="d-left-info">
                                                    <div class="d-pay-name">John Peter Doe</div>
                                                    <div class="d-pay-designation">
                                                        <div class="d-pay-pos">Cyberbacker to Josephene Bracken Doe</div>
                                                    </div>
                                                </div>
                                                <div class="d-right-info">
                                                    <div class="d-pay-range">Invoice number 1</div>
                                                    <div class="d-pay-date">November 16, 2022</div>
                                                </div>
                                            </div>
                                            <div class="d-pay-content">
                                                <div class="d-pay-earnings">
                                                    <div class="d-pay-item">
                                                        <div class="d-pay-label">SF for November 1 to 15</div>
                                                        <div class="d-pay-price">$540</div>
                                                    </div>
                                                </div>
                                                <div class="d-pay-deduction">
                                                    <div class="d-pay-item">
                                                        <div class="d-pay-label">Absense</div>
                                                        <div class="d-pay-price">- $10</div>
                                                    </div>
                                                    <div class="d-pay-item">
                                                        <div class="d-pay-label">CB Merch</div>
                                                        <div class="d-pay-price">- $60</div>
                                                    </div>
                                                    <div class="d-pay-item">
                                                        <div class="d-pay-label">HMO 50%</div>
                                                        <div class="d-pay-price">- $20</div>
                                                    </div>
                                                </div>
                                                <div class="d-pay-total">
                                                    <div class="d-pay-title">Total</div>
                                                    <div class="d-pay-numbers">450</div>
                                                </div>
                                            </div>
                                        </div>
                                    </v-card-text>

                                    <v-divider></v-divider>

                                    <v-card-actions>
                                        <v-spacer></v-spacer>
                                        <button>Send a copy to CB</button>
                                        <v-btn color="primary" text @click="dialog = false">
                                            I accept
                                        </v-btn>
                                    </v-card-actions>
                                </v-card>
                            </v-dialog>

                            <div class="d-payslip-history">
                                <div class="d-phistory-items">
                                    <div class="d-phistory-item" v-on:click="openSpecificPayslip()">
                                        <div class="d-ph-inv-number">12</div>
                                        <div class="d-ph-inv-from">November 1, 2022 to November 15, 2022</div>
                                        <div class="d-ph-inv-total">$450</div>
                                    </div>
                                    <div class="d-phistory-item">
                                        <div class="d-ph-inv-number">12</div>
                                        <div class="d-ph-inv-from">November 1, 2022 to November 15, 2022</div>
                                        <div class="d-ph-inv-total">$450</div>
                                    </div>
                                    <div class="d-phistory-item">
                                        <div class="d-ph-inv-number">12</div>
                                        <div class="d-ph-inv-from">November 1, 2022 to November 15, 2022</div>
                                        <div class="d-ph-inv-total">$450</div>
                                    </div>
                                    <div class="d-phistory-item">
                                        <div class="d-ph-inv-number">12</div>
                                        <div class="d-ph-inv-from">November 1, 2022 to November 15, 2022</div>
                                        <div class="d-ph-inv-total">$450</div>
                                    </div>
                                    <div class="d-phistory-item">
                                        <div class="d-ph-inv-number">12</div>
                                        <div class="d-ph-inv-from">November 1, 2022 to November 15, 2022</div>
                                        <div class="d-ph-inv-total">$450</div>
                                    </div>
                                    <div class="d-phistory-item">
                                        <div class="d-ph-inv-number">12</div>
                                        <div class="d-ph-inv-from">November 1, 2022 to November 15, 2022</div>
                                        <div class="d-ph-inv-total">$450</div>
                                    </div>
                                    <div class="d-phistory-item">
                                        <div class="d-ph-inv-number">12</div>
                                        <div class="d-ph-inv-from">November 1, 2022 to November 15, 2022</div>
                                        <div class="d-ph-inv-total">$450</div>
                                    </div>
                                    <div class="d-phistory-item">
                                        <div class="d-ph-inv-number">12</div>
                                        <div class="d-ph-inv-from">November 1, 2022 to November 15, 2022</div>
                                        <div class="d-ph-inv-total">$450</div>
                                    </div>
                                </div>
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
        name: 'CPayslip',
        data () {
            return {
                dialog: false
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

    .d-header-part {
        margin-bottom: 25px;
    }

    .d-header-part .d-left-info {
        width: 49%;
        display: inline-block;
        vertical-align: top;
    }

    .d-header-part .d-right-info {
        width: 49%;
        display: inline-block;
        vertical-align: top;
        text-align: right;
    }

    .d-pay-content .d-pay-content-title {
        background: #d5d5d5;
        padding: 10px 15px;
        text-align: left;
        text-transform: uppercase;
        margin-bottom: 15px;
        font-weight: bold;
    }

    .d-pay-item .d-pay-label {
        display: inline-block;
        width: 65%;
        vertical-align: top;
    }

    .d-pay-item .d-pay-price {
        display: inline-block;
        width: 34%;
        vertical-align: top;
        text-align: right;
    }

    .d-pay-item {
        margin-bottom: 15px;
        padding: 0 15px 15px;
        border-bottom: 1px solid #c7c7c7;
    }

    .d-payslip {
        border: 3px dashed #c3c3c3;
        padding: 20px;
        border-radius: 10px;
        margin-bottom: 15px;
    }

    .d-pay-total {
        padding: 0 15px;
    }

    .d-pay-total .d-pay-title {
        display: inline-block;
        width: 65%;
        vertical-align: middle;
        font-size: 18px;
        font-weight: bold;
    }

    .d-pay-total .d-pay-numbers {
        display: inline-block;
        width: 34%;
        vertical-align: middle;
        text-align: right;
        font-size: 18px;
        font-weight: bold;
    }
    .d-pay-name {
        font-size: 26px;
        font-weight: bold;
    }
    .d-logo-here {
        margin-bottom: 20px;
    }

    .d-logo-here > img {
        width: 250px;
    }

    .d-phistory-item{
        cursor: pointer;
        border: 1px solid #333;
        margin-bottom: 10px;
        padding: 10px;
        border-radius: 10px;
    }

    .d-phistory-item > div {
        display: inline-block;
        vertical-align: middle;
    }

    .d-phistory-item .d-ph-inv-number {
        width: 5%;
        text-align: center;
        font-weight: bold;
    }

    .d-phistory-item .d-ph-inv-from {
        width: 74%;
        font-style: italic;
    }

    .d-phistory-item .d-ph-inv-total {
        width: 20%;
        text-align: right;
        font-size: 18px;
        font-weight: bold;
    }

    
  </style>
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
                            <ProfileStats />
                            <ProfileSchedule />
                            <ProfileAttendance />
                            show activity here
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'CbProfile'
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

    
  </style>
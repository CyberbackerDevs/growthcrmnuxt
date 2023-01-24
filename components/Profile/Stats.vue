<template>
    <div class="d-profile-stats">
        <div class="d-stats-inner">
            <div class="d-stats-item">
                <div class="d-stats-number">
                    <span class="d-st-number">14</span>
                    <span class="d-st-text">Working Days</span>
                    <span class="d-st-range">Nov. 1 to Nov. 15, 2022</span>
                </div>
                <div class="d-stats-desc">
                    <button>View Details</button>
                </div>
            </div>
            <div class="d-stats-item">
                <div class="d-stats-number">
                    <span class="d-st-number">14</span>
                    <span class="d-st-text">Present</span>
                    <span class="d-st-range">Nov. 1 to Nov. 15, 2022</span>
                </div>
                <div class="d-stats-desc">
                    <button>View Details</button>
                </div>
            </div>
            <div class="d-stats-item">
                <div class="d-stats-number">
                    <span class="d-st-number">14</span>
                    <span class="d-st-text">Late</span>
                    <span class="d-st-range">Nov. 1 to Nov. 15, 2022</span>
                </div>
                <div class="d-stats-desc">
                    <button>View Details</button>
                </div>
            </div>
            <div class="d-stats-item">
                <div class="d-stats-number">
                    <span class="d-st-number">14</span>
                    <span class="d-st-text">Absenses</span>
                    <span class="d-st-range">Nov. 1 to Nov. 15, 2022</span>
                </div>
                <div class="d-stats-desc">
                    <button>View Details</button>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .d-profile-stats {
        margin-bottom: 20px;
        text-align: center;
    }
    .d-stats-item {
        display: inline-block;
        width: 22%;
        margin: 0 1%;
        border: 1px solid #4a4a4a;
        border-radius: 5px;
        text-align: left;
    }
    .d-stats-desc button {
        width: 100%;
        background: #4a4a4a;
        color: #fff;
        text-transform: uppercase;
        font-weight: 100;
        font-size: 16px;
        padding: 13px;
    }
    .d-stats-number > span {
        display: block;
    }
    .d-stats-number {
        padding: 20px 20px;
    }
    .d-stats-number span.d-st-number {
        font-size: 43px;
        font-weight: 700;
        line-height: 1em;
    }
</style>
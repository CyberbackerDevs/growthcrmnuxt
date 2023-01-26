<template>
    <div class="d-client-single">
        <div class="card mb-8">
            <div class="card-body pt-9 pb-0">
                <ClientHeader />
            </div>
        </div>

        <ClientRoadmap v-if="current_page == 'roadmap'" />
        
        <ClientOverview v-if="current_page == ''" />
    </div>
</template>

<script>
    export default {
        name: 'ClientSingle',
        data () {
            return {
				current_page: ''
            }
        },
        methods: {
			getClientPage(){
                this.current_page = this.$route.query.page
            }
        },
        mounted: function(){
            this.getClientPage();
        }
    }
</script>


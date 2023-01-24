<<template>
    <div class="d-client-all">
        <clientSingle />
        

    </div>
</template>

<script>
    export default {
        name: 'prepayDashboard',
        data () {
            return {
				selectedTab: 'current_roadmap',
                prepay_id: ''
            }
        },
        methods: {
			hasPtoId(){
                // console.log('has id -> ', this.$route.query);
                this.prepay_id = this.$route.query.id
            },
        },
        mounted: function(){
            this.hasPtoId();
        }
    }
</script>
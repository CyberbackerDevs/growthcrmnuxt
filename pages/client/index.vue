<<template>
    <div class="d-client-all">
        <clientSingle v-if="is_single" />
        
        <ClientList v-if="!is_single" />

    </div>
</template>

<script>
    export default {
        name: 'prepayDashboard',
        data () {
            return {
				is_single: '',
                prepay_id: ''
            }
        },
        methods: {
			hasPtoId(){
                console.log('has id -> ', this.$route.query.id);
                
                if(typeof(this.$route.query.id) !== 'undefined'){
                    this.is_single = true;
                } else {
                    this.is_single = false;
                }
            },
        },
        mounted: function(){
            this.hasPtoId();
        }
    }
</script>
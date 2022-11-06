<template>
    <div>
        <select v-model.number="n">
			<option value="1">1</option>
			<option value="2">2</option>
			<option value="3">3</option>
		</select>&nbsp;
        <p>{{sum}}</p>
        <p>{{name}}</p>
        <p>{{bigSum}}</p>
        <div>
            <button @click="JIA(n)">click</button>
            <button @click="jia(n)">click</button>
        </div>
    </div>
</template>
<script>
import {mapActions,mapGetters,mapMutations,mapState} from 'vuex'
export default {
    name:'Count',
    data() {
        return {
            n:1
        }
    },
    mounted() {
        
    },
    computed: {
        ...mapState(['sum','name']),
        ...mapGetters(['bigSum'])
    },
    methods: {
        ...mapMutations(['JIA']),
        ...mapActions(['jia'])
    },
}
</script>
<style>
    
</style>
<template>
    <div class="user-info">
        <div>
            User information
        </div>
        <div v-if="userInformation">
            <div>{{userInformation.userName}}</div>
            <div>{{userInformation.id}}</div>
            <div>{{userInformation.age}}</div>
        </div>
    </div>
</template>
<script>
export default {
    data(){
        return{
            userInformation: null
        }
    },
    created(){
        this.userInformation = this.getUserInformation(this.$route.params.id)
    },
    methods:{
        getUserInformation(id){
            console.log(id)
            return {userName: 'lucnd', id: "user00" + id, age: '23'}
        }
    }
}
</script>

<style scoped>
    .user-info{
        font-family: 'Times New Roman', Times, serif;
        font-size: 20px;
        font-weight: bold;
    }
</style>
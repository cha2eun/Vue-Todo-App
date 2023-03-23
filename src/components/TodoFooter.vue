<template>
    <div class="clearAllContainer">
        <span class="clearAllBtn" v-on:click="clearTodo">전체 삭제</span>
    </div>
</template>

<script>
export default{
    methods:{
        clearTodo: function(){
            localStorage.clear();
            window.location.reload(true);
        }
    }
}
</script>

<style scoped>
.clearAllContainer{
    width           : 8.5rem;
    height          : 50px;
    line-height     : 50px;
    background-color: white;
    border-radius   : 5px;
    margin          : 0 auto;
}
.clearAllBtn {
    color           : #e20303;
    display         : block;
    font-weight     : 900;
    font-size       : 20px;
}
</style>

<template>
    <div>
        <h3>There are fruits:{{a}},{{b}},{{c}}.</h3>
    </div>
</template>

<script>
    export default {
        // props使用数组接受父组件的传值
        // props:['a','b','c']

        //props使用对象接受父组件的传值
        props:{
            //参数的值可以配置
            a:{
                type:String,
                required:true
            },
            //validator
            b:{
                type:String,
                validator: function(value){
                    return value.length > 10;
                }
            },
            c:String
        }
    }
</script>

<style lang="scss" scoped>

</style>
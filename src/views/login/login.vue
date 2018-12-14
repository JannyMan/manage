<template>
    <div id="login">
        <div class="box">
            <h1>用户登录</h1>
            <ul>
                <li>
                    <span>用户名：</span>
                    <span><input type="text" placeholder="输入用户名"></span>
                </li>
                <li>
                    <span>密  码：</span>
                    <span><input type="text" placeholder="输入密码"></span>
                </li>
            </ul>
            <span id="sumbit" v-on:click="sumbit">登录</span>
            <span id="reset">重置</span>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'App',
        methods: {
            sumbit: function(){
                this.$router.push('/')
            }
        }
    }
</script>

<style lang="less" scoped>
   #login{
       width: 100%;
       height: 100%;
       background: Cyan;
       position: relative;
       .box{
           background: skyblue;
           width: 350px;
           height: 200px;
           position: absolute;
           left: 50%;
           top: 50%;
           margin-left: -175px;
           margin-top: -100px;
           h1{
               text-align: center;
           }
           #sumbit{
               background: orange;
               cursor: pointer;
           }
       }
   }
</style>

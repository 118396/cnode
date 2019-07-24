<template>
    <div class="header">
        <router-link :to="{name:'root'}">
        <img src="../assets/cnodejs_light.svg" alt="">
        </router-link>
        <ul>
            <li>
                <router-link :to="{name: 'root'}">首页</router-link>
            </li>
            <li>
                <router-link :to="{name: 'about'}">关于</router-link>
            </li>

        </ul>
    </div>
</template>

<script>
export default {
    name:"Header"
}
</script >
// scope:样式只对当前组件有效，如果去掉 scope ，对整个应用都有效
<style scoped> 
    .header{
        background-color: #5a5555;
        height: 50px;
    }
    img{
        max-width: 120px;
        margin-left:50px ;
        margin-top: 10px;
    }
    ul{
        list-style: none;
        float: right;
        margin: 4px;
    }
    li{
        display: inline-block;   
        padding: 10px 15px;
    }
    a{
        text-decoration: none;
        color: #ccc;
        font-size: 14px;
        text-shadow: none;
    }
</style>

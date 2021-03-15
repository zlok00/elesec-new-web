<template>
    <div class="header">
        <div class="wrap clearfix">
            <a href="index.html" class="logo"><img src="images/logo.jpg" alt="青寕信安" width="170" height="64"></a>
            <ul class="nav">
                <li :class="[num==1 ? 'curr' : '']"><a href="##">技术核心</a></li>
                <li :class="[num==2 ? 'curr' : '']"><a href="##">行业方案</a></li>
                <li><a href="##">商业案例</a></li>
                <li :class="[num==4 ? 'curr' : '']"><a href="news.html" target="_blank">新闻中心</a></li>
                <li :class="[num==5 ? 'curr' : '']"><a href="joinUs.html" target="_blank">加入我们</a></li>
                <li :class="[num==6 ? 'curr' : '']"><a href="about.html" target="_blank">关于我们</a></li>
            </ul>
        </div>
    </div>
</template>

<script>
    module.exports = {
        props:['keynumber'],
        data(){
            return {
              //  tabnum:1
                num: this.keynumber
            }
        },
        mounted(){
            console.log(this.num)
        }
    }
</script>

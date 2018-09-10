<template>
        <div class="home">
            <div class="bg-img">
                <div class="box">
                    <p class="bg_img_title">PAWN ' s Blog</p>
                    <hr/>
                    <p class="bg_img_dest">分享前端技术，学习前端知识！</p>
                </div>
            </div>
            <div class="container">
                <div class="content-left">
                    left
                </div>        
                <div class="content-right">
                    <Aside/>
                </div>
            </div>
        </div>
</template>

<script>
    import Aside from '../components/Aside.vue'
    export default {
        name: 'Home',
        data() {
            return {
                msg: ''
            }
        },
        components:{
            Aside
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="less" type="text/less" scoped>
    .home {
    
        .bg-img {
            width: 100%;
            background-image: url(/static/img/bg.jpg);
            background-position: 50%;
            height: 350px;
            background-size: 100% auto;
            margin-bottom: 40px;
            color: #fff;
            text-align: center;
            .box {
                position: relative;
                top: 40%;
                .bg_img_title {
                    font-size: 36px;
                    font-weight: bold;
                }
                hr {
                    width: 120px;
                    margin: 0 auto;
                }
                .bg_img_dest {
                    font-size: 16px;
                }
            }
        }
        .container{
            width: 1250px;
            margin: 0px auto;
            height: 200px;
            .content-left{
                float: left;
                width:900px;
                background-color:  blueviolet;
            }
            .content-right{
                float: right;
                width: 300px;
            }
        }
    }
</style>
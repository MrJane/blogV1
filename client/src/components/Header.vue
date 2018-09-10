<template>
  <nav class="header">
   <div class="container">
      <div  class="logo">
        <img src='../../static/img/logo.png'>
      </div>
      <ul class="nav_list">
          <li class="nav_item"><router-link to="/home">首页</router-link></li>
          <li class="nav_item"><router-link to="/production">作品</router-link></li>
          <li class="nav_item"><router-link to="/archives">归档</router-link></li>
          <li class="nav_item"><router-link to="/about">关于</router-link></li>
        </ul>
   </div>
  </nav>
</template>

<script>
    export default {
        name: 'Header',
        data() {
            return {
                msg: 'Welcome to Your Vue.js App'
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="less" scoped>
    .header {
        width: 100%;
        height: 60px;
        position: fixed;
        top: 0;
        left: 0;
        line-height: 60px;
        background-color: rgba(0, 0, 0, .1);
        .container {
            position: relative;
            width: 1250px;
            margin: 0px auto;
            .logo {
                height: 60px;
                line-height: 60px;
                padding: 6px 0;
                img {
                    height: 48px;
                }
            }
            .nav_list {
                position: absolute;
                top: 0;
                right: 0;
                li {
                    list-style: none;
                    float: left;
                    color: #fff;
                    a {
                        padding: 0 15px;
                        transition: color .3s;
                        height: 60px;
                        line-height: 60px;
                        display: inline-block;
                        &.router-link-exact-active {
                            color: #62be93;
                        }
                        &:hover {
                            color: #62be93;
                        }
                    }
                }
            }
        }
    }
</style>
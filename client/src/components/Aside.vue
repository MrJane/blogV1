<template>
        <div class="aside">
           <div class="search-box">
               <input type="text" placeholder="搜索..."/>
               <i class="iconfont icon-iconfontzhizuobiaozhun22"></i>
           </div>
           <div class="intro-box">
                <p class="intro-title">简介</p>
                <p class="intro-item">萧皇后</p>
                <p class="intro-item" title="成都大学2016级计算机科学与技术">(CDU)2016级计算机科学与技术</p>
                <p class="intro-item"><a href="mailto:1052069088@qq.com" :title='"电子邮箱\n1. 1052069088@qq.com\n2. lichangyigod@gmail.com"' target="_blank">Email</a></p>
                <p class="intro-item"><a href="http://github.com/lichangyi" title="github搜索: LiChangyi" target="_blank">GitHub</a></p>
                <p class="intro-item"><a href="https://juejin.im/user/59eeff42f265da43070275e1" title="掘金搜索: Pawn2018" target="_blank">掘金</a></p>
           </div>
           <div class="category-box">
               <p class="category-title">文章分类</p>
               <p class="category-item" title="查看全部">ALL</p>
               <p class="category-item">血腥大唐</p>
               <p class="category-item">血腥大唐</p>
               <p class="category-item">血腥大唐</p>
               <p class="category-item">血腥大唐</p>
           </div>
        </div>
      </template>

<script>
    export default {
        name: 'Aside'
    }
</script>

<style lang="less" scoped>
    .aside {
        .search-box {
            position: relative;
            input {
                display: block;
                width: 100%;
                height: 44px;
                box-sizing: border-box;
                padding: 8px 46px 8px 20px;
                outline: 0;
                color: inherit;
                border: none;
                border-radius: 22px;
                background-color: rgba(164, 177, 191, .15);
                box-shadow: none;
                transition: box-shadow .3s;
                &:hover,
                &:focus {
                    box-shadow: inset 0 0 0 2px #353030;
                }
            }
            i {
                position: absolute;
                top: 50%;
                right: 12px;
                transform: translateY(-50%);
                font-size: 20px;
                color: #353030;
            }
        }
        .intro-box {
            width: 100%;
            .intro-title {
                padding-left: 20px;
                font-size: 16px;
                border-left: 4px solid #62be93;
                margin: 30px auto 40px;
            }
            .intro-item {
                font-size: 14px;
                color: #666;
                text-align: center;
                line-height: 2;
            }
        }
        .category-box{
            width: 100%;
            .category-title{
                padding-left: 20px;
                font-size: 16px;
                border-left: 4px solid #62be93;
                margin: 30px auto 40px;
            }
            .category-item{
                font-size: 14px;
                line-height: 2;
                color: #666;
                text-align: center;
            }
        }
    }
</style>
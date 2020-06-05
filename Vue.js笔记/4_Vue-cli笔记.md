# 1.什么是Vue CLI

![](_v_images/20200601155504221_19937.png)
# 2.安装vue cli的前提
![](_v_images/20200601155816643_884.png)
![](_v_images/20200601155915185_26195.png)
# 3.Vue CLI的安装

![](_v_images/20200601161155238_1535.png)
经测试,我自己的window10电脑上需要使用 
```
vue.cmd --version
```
![](_v_images/20200601161533527_2129.png)

# 4.旧版本vue-cli2初始化项目

当前安装的是4.4版本，但是有些公司项目用的还是老的版本2版本，所以这里先要了解下旧版本的使用

![](_v_images/20200601161900739_28361.png)

![](_v_images/20200601164157135_8606.png)

![](_v_images/20200601163125775_32452.png)
ESLint:是否对js代码进行限制？
set up uint tests?   是否设置单元测试？
set up e2e tests with NightWatch?   端到端的测试？


![](_v_images/20200601164551465_10726.png)
![](_v_images/20200601164720075_5284.png)

# 5.vue-cli2的目录结构
![](_v_images/20200601170830217_28893.png)

# 6.安装CLI错误和ESLine规范

## 1.脚手架运行成功后默认的界面
![](_v_images/20200601200749908_11252.png)
![](_v_images/20200601200805384_12886.png)

# 7.理解 runtime-compiler和runtime-only的区别
![](_v_images/20200601221637172_30940.png)
![](_v_images/20200601221855447_29879.png)
![](_v_images/20200601221924555_15764.png)
*runtime-only比runtime-compiler要少6kb的代码量，性能上更好!*

![](_v_images/20200601222910311_28064.png)

上面这节适合多听几次！

https://www.bilibili.com/video/BV15741177Eh?p=95

# 8.npm run build的运行流程
![](_v_images/20200601223140325_15813.png)
![](_v_images/20200601223221381_27626.png)

# 9.给配置起别名
![](_v_images/20200601223317712_1902.png)
# 10.认识vue-cli3
![](_v_images/20200601223632925_32251.png)

创建项目
![](_v_images/20200601224402579_20023.png)
![](_v_images/20200601224811100_21580.png)
![](_v_images/20200601225049931_26206.png)
![](_v_images/20200601225505758_26919.png)
![](_v_images/20200601225823075_1027.png)

# 11.vue-cli4的目录结构
![](_v_images/20200601231836011_7994.png)

# 12.vue-cli4的配置文件查看和修改
![](_v_images/20200601232102865_18912.png)
![](_v_images/20200601234801843_22012.png)
![](_v_images/20200601234850533_19118.png)

# 13.知识点补充： ES6箭头函数与this指向



# 14.url的hash和html5的history



# 15.vue-router的安装和配置方式
![](_v_images/20200602163417231_709.png)



![](_v_images/20200602163143491_23731.png)
![](_v_images/20200602163251449_15124.png)

![](_v_images/20200602165825608_19302.png)

# 16.路由的默认值和修改为history模式

![](_v_images/20200602170045372_31194.png)
通过重定向的方式来实现
更改为history模式
![](_v_images/20200602170627188_24362.png)
![](_v_images/20200602170752568_37.png)

# 17.router-link的知识点补充
1.将router-link渲染成其他标签，通过tag属性
2.默认的路由使用history.pushState(),可以返回，如果不想返回，就需要改为history.replaceState(),   只需要加个replace属性就可以了
3.可以对激活状态的标签的active属性设置别名，通过 active-class

![](_v_images/20200602171856216_416.png)
![](_v_images/20200602171916160_2652.png)
![](_v_images/20200602172027657_22866.png)

# 18.通过代码跳转路由
![](_v_images/20200602172812496_16097.png)

vue-router提供了this.$router实例
* 1.this.$router.push(路由)            //可以返回
* 2.this.$router.replace(路由)        //不可以返回
* 3.this.$router.go(n)                   //前进或者后退几步
![](_v_images/20200602173630305_11539.png)

# 19.动态路由的使用
![](_v_images/20200602175229206_844.png)

![](_v_images/20200602181408950_26086.png)

![](_v_images/20200602181433125_30520.png)

# 20.路由懒加载的使用
![](_v_images/20200602184534470_7443.png)
![](_v_images/20200602184633132_20094.png)
![](_v_images/20200602185719275_32760.png)

# 21.认识嵌套路由
![](_v_images/20200602190204834_20038.png)

![](_v_images/20200602191210403_24412.png)


![](_v_images/20200602192922163_2959.png)

![](_v_images/20200602193142586_11844.png)

# 22.vue-router的参数传递

![](_v_images/20200602195109309_8031.png)
![](_v_images/20200602195554211_29561.png)
![](_v_images/20200602195713642_18808.png)
![](_v_images/20200602195744174_21571.png)

现在想要通过点击button按钮的方式进行跳转，并且传递参数
![](_v_images/20200602200631362_17017.png)

# 23.理解vue-router和route的由来(跳过了)

# 24.使用导航守卫


![](_v_images/20200603135548652_20078.png)

![](_v_images/20200603135735254_8586.png)

![](_v_images/20200603135802070_21696.png)


router.beforeEach()     被称为前置钩子,是在跳转之前进行的回调，也叫做钩子(hook)
router.afterEach()
都属于全局守卫

![](_v_images/20200603141634139_1001.png)
![](_v_images/20200603141725117_18754.png)


# 25.vue-router-keep-alive及其他问题
为了保存用户之前的路由状态，可以通过下面的方法

![](_v_images/20200603144935483_14635.png)

摘自博客 https://juejin.im/post/5c6e133ee51d455d06474a31
![](_v_images/20200603150006875_16448.png)
![](_v_images/20200603150041864_8839.png)
![](_v_images/20200603150109282_24913.png)
```
//生命周期：初始化阶段 运行中阶段 销毁阶段
    //html
     <div id="app">
        <app></app>
    </div>
    // js
    Vue.component("App",{
        template:`
            <div>
                <p class="myp">A组件</p>
                <button @click="destroy">destroy</button>
                <input type="text" v-model="msg">
                <p>msg:{{msg}}</p>
            </div>`,
        data:function(){
            return {msg:'hello'}
        },
        timer:null,
        methods:{
            destroy:function(){
                this.$destroy()//
            }
        },
        beforeCreate:function(){
            console.log('beforeCreate:刚刚new Vue()之后，这个时候，数据还没有挂载呢，只是一个空壳')           
            console.log(this.msg)//undefined
            console.log(document.getElementsByClassName("myp")[0])//undefined
        },
        created:function(){
            console.log('created:这个时候已经可以使用到数据，也可以更改数据,在这里更改数据不会触发updated函数')
            this.msg+='!!!'
            console.log('在这里可以在渲染前倒数第二次更改数据的机会，不会触发其他的钩子函数，一般可以在这里做初始数据的获取')
            console.log('接下来开始找实例或者组件对应的模板，编译模板为虚拟dom放入到render函数中准备渲染')
        },
        //created:() => {
            //这个写法this指向是有问题的 用箭头函数 this指向window 上面是对的
            //console.log('created:这个时候已经可以使用到数据，也可以更改数据,在这里更改数据不会触发updated函数')
            //this.msg+='!!!'
            //console.log('在这里可以在渲染前倒数第二次更改数据的机会，不会触发其他的钩子函数，一般可以在这里做初始数据的获取')
            //console.log('接下来开始找实例或者组件对应的模板，编译模板为虚拟dom放入到render函数中准备渲染')
        //},
        beforeMount:function(){
            console.log('beforeMount：虚拟dom已经创建完成，马上就要渲染,在这里也可以更改数据，不会触发updated')
            this.msg+='@@@@'
            console.log('在这里可以在渲染前最后一次更改数据的机会，不会触发其他的钩子函数，一般可以在这里做初始数据的获取')
            console.log(document.getElementsByClassName("myp")[0])//undefined
            console.log('接下来开始render，渲染出真实dom')
        },
        // render:function(createElement){
        //     console.log('render')
        //     return createElement('div','hahaha')
        // },
        mounted:function(){ 
            console.log('mounted：此时，组件已经出现在页面中，数据、真实dom都已经处理好了,事件都已经挂载好了')
            console.log(document.getElementsByClassName("myp")[0])
            console.log('可以在这里操作真实dom等事情...')

        //    this.$options.timer = setInterval(function () {
        //        console.log('setInterval')
        //         this.msg+='!'  
        //    }.bind(this),500)
        },
        beforeUpdate:function(){
            //这里不能更改数据，否则会陷入死循环
            console.log('beforeUpdate:重新渲染之前触发')
            console.log('然后vue的虚拟dom机制会重新构建虚拟dom与上一次的虚拟dom树利用diff算法进行对比之后重新渲染')         
        },
        updated:function(){
            //这里不能更改数据，否则会陷入死循环
            console.log('updated:数据已经更改完成，dom也重新render完成')
        },
        beforeDestroy:function(){
            console.log('beforeDestory:销毁前执行（$destroy方法被调用的时候就会执行）,一般在这里善后:清除计时器、清除非指令绑定的事件等等...')
            // clearInterval(this.$options.timer)
        },
        destroyed:function(){
            console.log('destroyed:组件的数据绑定、监听...都去掉了,只剩下dom空壳，这里也可以善后')
        }
    })


    
    new Vue({
        el:'#app'
    })
```

# 26.vue生命周期钩子函数actived没有执行？
![](_v_images/20200603150324200_20354.png)
![](_v_images/20200603150345297_13040.png)
![](_v_images/20200603150405657_13717.png)
![](_v_images/20200603150753595_16911.png)

***注意点：只有使用了keep-alive,才可以使用  activated/deactivated  ,否则是不会触发的***

# 27.vue-router-keep-alive属性介绍，可以指定哪些不会被缓存
![](_v_images/20200603151500457_19926.png)
![](_v_images/20200603151900335_2960.png)

# 28.tabbar的封装(小案例)
![](_v_images/20200603152534610_4386.png)

## 1.tabbar基本结构的搭建
![](_v_images/20200603192328037_24154.png)
传统的思想，是将这个tabbar直接在App组件中编码渲染出来.但是Vue是组件化的思想，并不是这样搞的，这样搞不利于后期的代码维护！
下面对代码进行重新架构！
## 2.对tab-bar和tab-bar-item进行封装
用到的技术点：
1.插槽的使用

新建一个TabBar组件，将代码从App组件中抽离出去
![](_v_images/20200603194658862_20058.png)

最终完成的代码演示

![](_v_images/20200604140943628_9491.png)
![](_v_images/20200604141246017_10366.png)

# 29.给路径设置别名
vue-cli4没有找到相关的配置方法


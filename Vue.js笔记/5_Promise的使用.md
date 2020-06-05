# 1.promise的介绍
![](_v_images/20200604142616345_9202.png)

## 1.回调地狱
当网路请求非常复杂的时候，就会出现回调地狱。
![](_v_images/20200604143329652_13419.png)

使用Promise解决
# 2.Promise的介绍
![](_v_images/20200604143737968_32436.png)

## 1.什么情况下会用到Promise?
一般情况下是异步操作时，使用Promise对这个异步操作进行封装
![](_v_images/20200604151515003_24616.png)

## 2.promise的三种状态
![](_v_images/20200604152442856_21306.png)

三种状态:
pending:等待状态
fulfill:满足状态    ，会调用.then
rejected：拒绝状态   ,会调用  .catch

## 3.Promise的另外一种处理形式
![](_v_images/20200604153741264_19370.png)
## 4.Promise的链式调用
![](_v_images/20200604154107035_30736.png)

![](_v_images/20200604160145076_11182.png)
![](_v_images/20200604160221342_14486.png)

# 3.Promise的all方法的使用
该方法针对于  同时几个请求都执行完毕之后才开始进行的操作！

![](_v_images/20200604161049982_25603.png)

Promise.all( 请求数组列表).then( res => {
    console.log( res )
})
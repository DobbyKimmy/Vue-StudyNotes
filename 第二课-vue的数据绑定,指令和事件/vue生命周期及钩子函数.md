## vue生命周期及钩子函数
1. beforeCreate()

       vue实例初始化调用;el,data这些属性值均为undefinded
       
       
2. created()

       vue实例创建完成后调用,当尚未挂载到DOM元素上;el还是undefined
       但是数据已经与data中的属性进行了绑定    

3. beforeMount()
    
        beforeMount指的是载入前,在这个周期vue完成了data和el数据的初始化
        但是页面的内容还是vue的占位符
        
4. mounted()

        el(刚刚)已经挂载到了DOM元素上

5. beforeUpdate(),updated()

        beforeUpdate和updated都是view层数据变化才会触发的,
        如果仅仅是data中的数据改变无法触发。
        
        beforeUpdate: 重新渲染页面之前触发
        updated: 数据已经更改,DOM也重新render

6. beforeDestroy()

        vue实例销毁前执行,如清除计时器等等
        
7. destroyed()

        vue实例销毁后执行        

## vue中的基本指令

#### v-cloak 
````
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>v-clock</title>
    <style>
        [v-cloak]{
            display: none;
        }
    </style>
</head>
<body>
<div id="app">
    <!--v-cloak:解决页面加载缓慢导致页面出现闪动,要与display:none一同使用-->
    <span v-cloak>{{msg}}</span>
</div>
<script src="https://cdnjs.cloudflare.com/ajax/libs/vue/2.6.10/vue.min.js"></script>
<script>
    var app = new Vue({
        el:'#app',
        data:{
            msg:'vue is cool!'
        }
    })
</script>
</body>
</html>
````

#### v-once
````
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>v-once</title>
</head>
<body>
<div id="app">
    <!--v-once:定义了v-once的元素或组件只渲染一次-->
    <span v-once>{{msg}}</span>
</div>
<script src="https://cdnjs.cloudflare.com/ajax/libs/vue/2.6.10/vue.min.js"></script>
<script>
    var app = new Vue({
        el:'#app',
        data:{
            msg:'vue is cool!'
        }
    })
</script>
</body>
</html>
````

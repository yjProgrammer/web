# web
vue.js
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>
    <div id="app">
        <!--{{}}用于标签体内显示数据-->
        Hello,{{msg}}<br/>
        <!--v-model进行数据的双向绑定-->
        <input type="text" v-model="msg"> 
    </div>

    <script src="./node_modules/vue/dist/vue.js"></script>
    <script>
    new Vue({
        el:'#app',//指定被Vue管理的入口，值为选择器，不可以指定body和html
        data() {  // 用于初始化数据，在Vue实例管理的Dom节点下，可通过末班请求来引用
            return {
                msg:'Vue.js'
            }
        }
    })
    </script>
</body>
</html>

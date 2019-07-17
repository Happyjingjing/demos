# demos
VUE学习：

<script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>

追加新数组： 

push()  pop()  shift()   unshift()   splice()  sort()  reverse()

Vue.set(vm.newsList,7,{title:'123',new:true,id:7})

vm.$set(vm.newsList,8,{title:'这是第八个',new:false,id:1})

vm.newsList.splice(9, 1, {title:'第九个'})


v-show :display:none   v-if: 移除元素



v-on:修饰符：

.stop   .prevent  capture  .self  .once  .passive


保存切换input中的值不变：

        <keep-alive>
            <component :is="type" ></component>
        </keep-alive>


<script>
        const cmpOne = {
            template:`<div>组件1：<input type="value"></div>`
        }
        const cmpTwo = {
            template:`<div>组件2：<input type="value"></div>`
        }
        new Vue({
            el:'#app',
            components:{
                cmpOne,
                cmpTwo
            },
            data:{
                showOne:true,
                type:'cmp-one'
            },
            methods:{
                changeCmp(){
                    // this.showOne = !this.showOne;
                    this.type = this.type == 'cmp-one' ? 'cmp-two' : 'cmp-one'
                }
            }
        })

    </script>



vue生命周期：onload onshow onready


vue-cli 学习：

命令：

npm install -g @vue/cli  //安装vue-cli

vue --version  // 查看vue-cli 版本

vue create 文件名  //创建文件

code .   // 打开文件(在vscode)

npm run serve  //运行 vue


运行单个vue文件：

vue serve 文件

npm install -g @vue/cli-service-global

cd src
cd components

vue serve 文件


创建vue项目：(图形界面)

vue ui


vue3 退回 vue2  :

npm install -g @vue/cli-init

vue init webpack my-project


vue路由：

vue add router  //路由安装


用户代码片段： ctrl+shift+p

文件--首选项--用户代码片段-- vue  打开vue.json

scoped ： 样式独立

vuex 安装： vue add vuex
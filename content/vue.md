##### vue
    1. vue的简介
        -特点
            --渐进式

    2. vue的简单使用
        -数据驱动视图
            --js版   --Exercise01.html
            --vue版  --Exercise02.html

    3. vue的指令
        -v-if   --Exercise03.html

        -v-show --Exercise04.html
            --通过style=display属性来控制显示或隐藏

        -v-for  
            --遍历数组或对象  --Exercise05.html
            key是用来给每一项值加元素标识，作用是为了区分元素，为了实现最小量的更新??????
            --遍历JSON  --Exercise06.html
            --嵌套遍历  --Exercise07.html

        -v-text/v-html  --Exercise08.html
            --{{}}、v-text、v-html的区别与联系
            联系：双大括号和v-text渲染结果类似，都是会以文本类型进行渲染
            区别:  1)双大括号在渲染结果之前，会有编译之前的文本显示，v-text是没有这种现象的
                  2)双大括号更灵活，中间是可以添加内容的，v-text是只能渲染data中的数据，中间不允许插入内容
                  3)v-html会识别模板

        -v-cloack   --Exercise09.html
        
        -v-once --Exercise10.html
            --对视图的元素渲染一次，数据更新不会引起视图的更新，目的是为了优化页面的性能
        
        -v-pre  --Exercise11.html
            --作用:跳过该元素编译过程，直接显示元素内部的文本，特点就是跳过大量的没有指令的节点

        -v-on  --Exercise12.html
            --vue的监听事件的语法：使用是一律去除原生js监听事件的前缀on，然后 添加v-on:事件名称或者@事件名称
        
        -v-bind 
            --作用：将普通的w3c属性变为动态属性，让属性具有动态能力
            --v-bind的语法  --Exercise13.html
            --v-bind使用class实现动态加载   --Exercise14.html
            --v-bind使用style实现动态传值加载  --Exercise15.html

        -v-model
            --作用：使用在表单元素中，实现表单和数据的双向绑定
            --v-model调查表单练习       --Exercise16.html
        
    4. 案例
       -选项卡练习   --Exercise17.html
       -调色板       --Exercise18.html
       -微博发布框   --Exercise19.html

    5. 修饰符
        -事件修饰符
            --事件冒泡是如何产生的？ --Exercise20.html
            --阻止事件冒泡的修饰符
                (1).stop        --Exercise21.html
                (2).self        --Exercise22.html
            --.prevent          --Exercise23.html
            --.capture          --Exercise24.html
            --.once             --Exercise25.html
        
        -按键修饰符
            --按键修饰符的使用      --Exercise26.html
            --常用的按键修饰符
            keyCode值	别名	键盘按键
                13	    .enter	回车
                32	    .space	空格
                37	    .left	键盘左键
                38	    .up	    键盘上键
                39	    .right	键盘右键
                40	    .down	键盘下键
                9	    .tab	键盘tab
                46或者8	.delete	delete或者backspace
        
        -系统修饰符
            --系统修饰符的使用      --Exercise27.html
            --常用的系统修饰符
            修饰符名称	对应的键盘键名称
            .ctrl	    ctrl
            .alt	    alt
            .shfit	    shift
            .meta	    如果是windows系统代表的是键盘的徽标键，如果是IOS系统，单表的是common键
            .exact      辅助其他修饰符进行精确匹配

        -鼠标按键修饰符
            --鼠标按键修饰符的使用      --Exercise28.html

        -表单修饰符
            --.lazy,.trim,.number             --Exercise29.html

    6. VUECli
        -install流程：https://cli.vuejs.org/guide/installation.html

        -cli目录结构

        -vue的起步文件
            --main.js
            --public/index.html
            --src/App.vue
        
        -组件
            --组件使用初体验        --Hello.vue
            --如何使用组件？
        
        -父子组件传值
            --原理：父组件通过v-bind自定义属性传入值，子组件通过props接受对应的参数
            --父子组件传值的使用
                (1) props接受单个值   --Exercise01.vue
                (2) props使用数组或者对象接受多个值  --Exercise02.vue
                (3) 子组件修改父组件的值   --Exercise03.vue






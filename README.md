# RelearnGit🤣🤣

### 默认参数的临时死区✔

这里的参数不可访问，与let声明类似，定义参数时会为每个参数创建一个新的标识符绑定，该绑定在初始化之前不会被引用，如果视图访问会导致程序抛出错误。当调用函数时，会通过传入的值或参数的默认值初始化该参数。

`function add(first = seconde, second) {`

​	`return first + second;`

`}`

`console.log(add(1 + 1));        //2`

`console.log(add(undefined, 1));   //抛出错误`

### 解析✔

在这个示例中，`add(1, 1)`时的代码用JavaScript表示为

`let first = 1`

`let second = 1`



`add(undefiend, 1)`时的JavaScript代码

`let first = second`

`let seconde = 1`

在这个示例中，调用 `add(undefiend, 1)`函数，当first初始化时second尚未初始化，所以会导致程序抛出错误，此时second尚处于临时死区中，正如let绑定时所说，所有引用临时死区中绑定的行为都会报错。



`注意：函数参数有自己的作用域和临时死区，其与函数体的作用域是各自独立的，就是说，参数的默认值不可访问函数体内声明的变量`；

create a new branch is quick and simple.

--no--ff 表示禁用Fast forward

i resolve the bug

hello
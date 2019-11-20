# RelearnGit

### 默认参数的临时死区✔

这里的参数不可访问，与let声明类似，定义参数时会为每个参数创建一个新的标识符绑定，该绑定在初始化之前不会被引用，如果视图访问会导致程序抛出错误。当调用函数时，会通过传入的值或参数的默认值初始化该参数。

`function add(first = seconde, second) {`

​	`return first + second;`

`}`

`console.log(add(1 + 1));        //2`

`console.log(add(undefined, 1));   //抛出错误`


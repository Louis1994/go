1. 自动垃圾回收机制GC
2. 丰富的内置数据类型：字典类型map、数据切片slice（语言内置特性，所以开发者根本不用费事去添加依赖的包，既可以少一些输入工作量）
3. 多返回值 例：func getName()(firstName, middleName, lastName, nickName string) {} 函数名 参数列表 返回值列表 函数体
4. 错误处理 defer、panic和recover关键字，避免大量的try-catch嵌套，减少代码量
5. 匿名函数和闭包 所有的函数也是值类型，可以作为参数传递
6. 类型和接口 只是支持最基本的类型组合功能，还引入了一个无比强大的“非侵入式”接口的概念，让开发者从以往对C++和Java开发中的接口管理问题中解脱出来
7. 并发编程 引入了goroutine概念，通过在函数调用前使用关键字go，我们即可让该函数以goroutine方式执行。goroutine是一种比线程更加轻盈、更省资源的协程。
    Go语言通过系统的线程来多路派遣这些函数的执行，使得每个用go关键字执行的函数可以运行成为一个单位协程。当一个协程阻塞的时候，调度器就会自动把其他协
    程安排到另外的线程中去执行，从而实现了程序无等待并行化运行。而且调度的开销非常小，一颗CPU调度的规模不下于每秒百万次，这使得我们能够创建大量的
    goroutine，从而可以很轻松地编写高并发程序
8. 反射 

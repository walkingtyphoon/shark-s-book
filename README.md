# C++基础



1. ### 引用和指针的区别是什么？
   1. **从语法和操作的角度来讲**，引用语法更加简单，使用点来访问成员，不需要使用解引用操作符；指针语法相对繁琐，需要使用`->`或者`*`来访问成员。
   2. **从安全的角度来讲**，引用更加安全，因为引用必须在声明时初始化，且不能为空，指针可能存在空指针，需要在使用前进行判空操作。
   3. **从内存管理的角度来讲**，引用不需要像指针一样显式进行内存管理，指针需要手动管理内存，包括动态分配和释放。
   4. **从灵活性来讲**，引用一旦引用指向了某个变量，就不能再改变，而指针可以在运行时改变指向，更加灵活。
   5. **从使用场景角度来讲**，引用适用于函数参数传递和返回值，适合用在需要别名而非新建变量的场景。而指针适用于动态内存分配和释放，更加灵活，可以在运行时改变指向。
2.  ### `const`关键字的作用是什么？

    用于定义常量或者指明不可修改的变量，它可以用于修饰变量，函数参数，函数返回值等，提高代码的可读性和稳定性
3.  ### 什么是函数重载？

    函数重载是指在同一个作用域内，可以定义多个同名函数，但它们的参数类型或个数必须不同，编译器根据调用时提供的参数选择匹配的函数
4.  ### 什么是默认参数，如何在函数中使用默认参数？

    默认参数是在函数声明时为参数指定一个默认值，调用函数时如果没有提供相应的参数，就是用默认值，其默认值从右往左。
5.  ### 什么是析构函数，其作用是什么？

    构造函数用于初始化对象的数据成员，析构函数用于在对象生命周期结束时进行清理工作，析构函数的名称与类型相同，没有返回值类型，而析构函数的名称是在类名前加上波浪号`~`

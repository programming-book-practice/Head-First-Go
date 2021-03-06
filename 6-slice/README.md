要点  

■　同型的切片变量与数组变量的声明相同，只是它忽略了长度：  

```go
var mySlice []int
```

■　在大多数情况下，切片和数组的代码行为完全相同。包括元素赋值、使用0值、传递给len函数和for...range循环。  
■　切片字面量的声明与数组字面量相同，但它忽略了长度：  

```go
[]int{1,7,10}
```

■　你可以获取通过切片运算符s[i：j]获取切片中i到j-1的元素。  
■　os.Args包变量包含当前程序执行的命令行参数组成的string类型的切片。  
■　变长参数函数是可以被不同个数的参数调用的函数。  
■　为了声明一个变长参数函数，在最后一个参数之前增加省略号（...）。这个参数就可以以切片的形式接收一组参数。  
■　当调用可变参数函数的时候，可以通过在切片之后追加省略号的方式来代替变长参数：  

```go
inRange(1,10,mySlice...)
```


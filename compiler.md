* 指针有效运算
    * 相同类型指针之间的赋值运算
    * 指针同整数之间的加法减法运算
    * 指向同一个数组中元素的两个指针间的减法或比较运算
    * 指针赋值0或与0（NULL）的比较运算
* front end
    * scanning (source code to tokens)
    * parsing (tokens to ast)
    * semantic analysis (types match)
* optimizer
    * common subexpress elimatation (cse)
* back end
    * register allocation (mapping virtual registers into physic registers)
    * instruction scheduling (reorder instructions to reduce execution cycles)
    * instruction selection
* 运算符优先级：决定不同运算符之间如何优先执行，结合性：决定相同运算符之间如何优先执行。
* 
| Name       | Operators | Associates |
| ---------- | --------- | ---------- |
| Equality   | == !=     | Left       |
| Comparison | > >= < <= | Left       |
| Term       | - +       | Left       |
| Factor     | / *       | Left       |
| Unary      | ! -       | Right      |
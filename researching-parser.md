# Parser

## Parser generator中需要解决的问题：

| 问题            | ebnf                |
|---------------|---------------------|
| 递归            | expr: expr '+' expr |
| 左递归           | expr: expr ';'      |
| 右递归           | expr: '-' expr      |
| else悬空        |                     |
| epsilon       | ε                   |
| precedence    | '+' '*'             |
| associativity | '+' '*'             |
| 最长匹配原则        |                     |

是否存在可化简的表达式？
是否存在可快速匹配的表达式？如无|的表达式。
lookahead-k能起到什么作用？
backtracking

错误处理于错误恢复的原则是什么？

解算

当前状态的可解释性，以及多解释的优先级(最长匹配原则)。
绝对解释和二义性解释(多解释)
first集和follow集能发挥什么样的作用？

对终结符进行分类：

1. 只能是前缀(prefix)的运算符，如'+', '-'
2. 只能是中缀(infix)的运算符，如'+', '-', '*', '/'
3. 只能是后缀(suffix)的运算符，如'++', '--'

结合性：左递归是左结合，右递归是右结合。

ebnf的各种语法替代：
x+ -> t: tx | x
x* -> t: tx | x | ε
x? ->  :  x | ε

## ANTLR是LL(k)方法，能解决formal language的parsing





# 创建题解 - `lc`

## [1]. 获取今日题目 - [`-t`/`--today`]

在终端中键入`lc`指令，即可默认在当前终端的工作区中获取今日的题目。

```shell
lc
# 完整指令
lc -t
```

示例获取今日题目：

```shell
# 例如当前执行目录为src目录
➜  src git:(dev) ✗ lc
MODE: today
题目[2867.统计树中的合法路径数目]获取成功!
题目文件地址为:/home/wh131462/workspace/leetcode-practice/src/2867.count-valid-paths-in-a-tree/index.js
```

## [2]. 获取指定题目 - [`-i`/`--identity`]

在终端中键入`lc`指令加上对应的题号，即可在当前工作区中获取指定题目。

```shell
lc 1314
# 完整指令
lc -i 1314
# 使用双引号(")进行包裹 可以确保指定编号准确，对于带空格的题目编号尤其有用
lc -i "LCP 50"
```

示例获取`LCP 50`：

```shell
➜  src git:(dev) ✗ lc "LCP 50"
MODE: identity
题目[LCP 50.宝石补给]获取成功!
题目文件地址为:/home/wh131462/workspace/leetcode-practice/src/LCP 50.WHnhjV/index.js
```

## [3]. 获取随机题目 - [`-r`/`--random`]

在终端中键入`lc`指令加上参数`-r`，即可在当前工作区中获取随机题目，会优先获取不存在当前目录中的题目。

```shell
# 完整指令
lc -r
```

示例获取随机题目：

```shell
➜  src git:(dev) ✗ lc -r
MODE: random
题目[14.最长公共前缀]获取成功!
题目文件地址为:/home/wh131462/workspace/leetcode-practice/src/14.longest-common-prefix/index.js
```

## [4]. 简单创建模式(交互式创建) - [`-e`/`--easy`]

除了如上的使用精准的指令快速创建题目外，还可以使用简单创建模式来进行交互式创建。

```shell
lc -e
```

使用简单模式创建今日题目示例：

```shell
➜  src git:(dev) ✗ lc -e
? 请选择创建问题的模式: today
? 是否在目录[ /home/wh131462/workspace/leetcode-practice/src ]下创建题目[ 2867.count-valid-paths-in-a-tree ]? Yes
题目[2867.count-valid-paths-in-a-tree]创建完成！
文件地址为: /home/wh131462/workspace/leetcode-practice/src/2867.count-valid-paths-in-a-tree/index.js

```

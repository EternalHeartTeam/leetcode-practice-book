# 检查题解 - `lk`

## [1]. 检查今日题解 [`-t`/`--today`]

在终端中键入`lk`指令，即可在当前工作区中检查今日题解。

```shell
# 默认执行检查今日题解
lk
# 完整指令
lk -t
```

使用示例:

```shell
# 指定了src目录为根目录
workspace/leetcode-practice [dev●] » lk -d src -t
MODE: today
题目[2581.统计可能的树根数目]检测结果:
```

| index | 测量结果 | 预期结果 | 执行结果  | 执行用时 | 内存占用 |
| ----- | -------- | -------- | --------- | -------- | -------- |
| 0     | 未通过   | '3'      | undefined | 0.0921ms | 2.52 KB  |
| 1     | 通过     | '5'      | undefined | 0.0119ms | 2.66 KB  |

> 点击跳转到题目提交:<https://leetcode.cn/problems/count-number-of-possible-root-nodes/>

## [2]. 检查指定题解 [`-i`/`--identity` + `<identity>`]

在终端中键入`lk`指令,并输入题目编号，即可在当前工作区中检查指定题解。

```shell
# 检查指定题解
lk 2581
# 完整指令
lk -i 2581
# 带空格的编号 使用双引号包裹
lk "LCP 50"
```

使用示例检查指定题解:

```shell
workspace/leetcode-practice [dev●] » lk -d src 2581
MODE: identity
题目[2581.统计可能的树根数目]检测结果:
```

| index | 测量结果 | 预期结果 | 执行结果 | 执行用时 | 内存占用 |
| ----- | -------- | -------- | -------- | -------- | -------- |
| 0     | 通过     | '3'      | '3'      | 0.1668ms | 2.52 KB  |
| 1     | 通过     | '5'      | '5'      | 0.0234ms | 2.66 KB  |

> 点击跳转到题目提交:<https://leetcode.cn/problems/count-number-of-possible-root-nodes/>

## [3]. 检查随机获取的题解 [`-r`/`--random`]

在终端中键入`lk`指令,使用参数`-r`，即可在当前工作区中检查上一个随机获取的题解。

```shell
# 完整指令
lk -r
```

使用示例:

```shell
workspace/leetcode-practice [dev●] » lk -r
MODE: random
题目[41.缺失的第一个正数]检测结果:
```

| index | 测量结果 | 预期结果 | 执行结果  | 执行用时 | 内存占用 |
| ----- | -------- | -------- | --------- | -------- | -------- |
| 0     | 未通过   | '3'      | undefined | 0.0896ms | 2.42 KB  |
| 1     | 未通过   | '2'      | undefined | 0.0110ms | 2.56 KB  |
| 2     | 未通过   | '1'      | undefined | 0.0045ms | 2.56 KB  |

> 点击跳转到题目提交:<https://leetcode.cn/problems/first-missing-positive/>
>
> 注意:在执行此指令之前请务必先执行过,`lc -r`创建了随机题目。

## [4]. 简单模式(交互式检查) [`-e`/`--easy`]

在终端中键入`lk`指令,使用参数`-e`，即可使用交互式的进行题目检查。

```shell
# 完整指令
lk -e
```

使用简单模式检测指定题目:

```shell
workspace/leetcode-practice [dev●] » lk -e
? 请选择检查问题的模式: identity
? 请输入题目编号: 41
? 是否检测当前目录[ /Users/mac-106/wh131462/workspace/leetcode-practice ]下的题目[ 41.first-missing-positive ]? Yes
```

| index | 测量结果 | 预期结果 | 执行结果  | 执行用时 | 内存占用 |
| ----- | -------- | -------- | --------- | -------- | -------- |
| 0     | 未通过   | '3'      | undefined | 0.0969ms | 2.42 KB  |
| 1     | 未通过   | '2'      | undefined | 0.0139ms | 2.56 KB  |
| 2     | 未通过   | '1'      | undefined | 0.0051ms | 2.56 KB  |

> 点击跳转到题目提交:<https://leetcode.cn/problems/first-missing-positive/>
> 题目[41.first-missing-positive]检查完成！
> 文件地址为: /Users/mac-106/wh131462/workspace/leetcode-practice/41.first-missing-positive/index.js

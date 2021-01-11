## 命令格式

| iptables  [-t 表名]   命令选项  [链名] [条件匹配] [-j 执行动作] |
| ---- |

<table>
  <tr >
	    <td> </td>
      <td> </td>
	    <td>表名</td>
	    <td>命令选项</td>
      <td>链表</td>
      <td>参数</td>
      <td> </td>
      <td>执行动作</td>
	</tr>
	<tr >
	    <td rowspan="10">iptable</td>
      <td rowspan="10">-t</td>
	    <td rowspan="10">
        [filter]</br>
        [nat]</br>
        [mangle]</td>
	    <td rowspan="10">
        -A  [添加规则]</br>
        -D  [删除规则]</br>
        -I  [插入规则]</br>
        -R  [替换规则]</br>
        -L  [查看规则]</br>
        -F  [清空规则]</br>
        -P  [设置默认]</br>
      </td>
      <td rowspan="10">
        PREROUTING</br>
        INPUT</br>
        FORWARD</br>
        OUTPUT</br>
        POSTROUTING</br>
      </td>
      <td>
        -p</br>
        -p</br>
        -p</br>
        -p</br>
        -p</br>
        -p</br>
        -p</br>
        -p</br>
        -p</br>
        -p</br>
        -p</br>
        -p</br>
        -p</br>
        -p</br>
        -p</br>
      </td>
      <td>-j</td>
      <td>
        ACCEPT[接收]</br>
        DROP[丢弃]</br>
        REJECT[拒绝]
      </td>
	</tr>
  </table>
  
## 命令分类

### 规则管理

| 选项   | 功能  |
|  :----:  | ----  |
| -A  | 在指定链表的末尾添加(--append)一条新的规则 |
| -D | 删除(--delete)指定链表中的某一条规则，按照规则序号或者规则内容删除 |
| -I | 在指定位置插入(--insert)一条新规则，按照规则序号或者规则内容确定位置 |
| -R | 修改替换(--replace)指定链表中的一条规则，按照规则序号或者规则内容确定位置 |

### 规则查看

| 选项   | 功能  |
|  :----:  | ----  |
| -L | 列出(--list)指定链表中的所有规则，不指定链表则列出所有链表规则 |
| -n | 用数字形式(--numberic)显示输出结果，显示ip地址而不是主机名称 |
| -v | 显示详细(--verbose)的规则信息 |
| --line-number | 显示规则的行号 |

### 链表管理

| 选项   | 功能  |
|  :----:  | ----  |
| -P | 设定指定链表的默认策略(--policy) |
| -F | 清空(--flush)指定链表中的规则，不指定则清空所有链表规则 |
| -N | 新建(--new-chain)一条用户自定义的规则链表 |
| -X | 删除指定链表中用户自定义的规则(--delete-chain) |
| -Z | zero，清零，置零规则计数器 |
| -E | rEname，重命名用户自定义链；引用计数不为 0 的自定义链，无法改名，也无法删除 |


<kbd>ctrl</kbd>

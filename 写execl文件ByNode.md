# node 操作execl文件

## 输出execl ->xxx.xlsx

### 安装依赖插件

```javascript
npm install excel node-xlsx
```
### 代码

```javascript
var xlsx = require('node-xlsx');
var fs = require('fs');

var data = [['学号', '科目', '分数'], [20094071309, '语文', 100, '天才'], [20094071310, '语文', 60, '待挂'], [20094071317, '语文', 80, '嗯不错']];
var buffer = xlsx.build([{name: "xx班语文成绩", data: data}]); // returns a buffer
fs.writeFile('./resut.xlsx', buffer, function (err) {
  if (err) throw err;
  console.log('has finished');
});
```



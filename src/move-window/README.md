## 滑动窗口 ==>  查找最长子串

#### 分析
* 利用队列的特征：先进先出
* 遍历字符串，依次进入队列
* 判断当前字符是否在队列中，
  * 如果在队列中，就索引出该位置，并将队列的元素从开始当前位置的元素都出队列，并将下一个元素`push`进队列
  * 如果不在对列中，就`push`进队列，依次扩展队列
* 每次操作队列都记录一下队列的长度，并且和上一次长度对比，取最长。
  
  

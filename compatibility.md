## 兼容性问题记录

#### [2020-4-15] safari浏览器不支持`new Date('2020-04-01 00:00:00')`
- 解决方法：
  1. 将-（横杠）替换成/（斜杠），`new Date('2020-04-01 00:00:00'.replace(/-/g, '/'))`
  2. 在服务端处理好格式，避免在浏览器端使用new Date('xxx')

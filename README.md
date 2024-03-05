# interviewer

## 一小时场

- 自我介绍（印象分）
  - 寒暄
    - 为什么考研计算机方向
    - 为什么选择前端
- 项目（基础分） 10 min
  - 具体情况而定
- 八股（基础分，可以省略） 10 min
  - html 基础
  - js 基础
    - promise
      - https://juejin.cn/post/7151636219036696613
      - https://www.zhihu.com/question/268007969
      - https://juejin.cn/post/6844904079353708557
      - https://juejin.cn/post/6844903858129338375
      - 
      ```js
      requestAnimationFrame(function onAf() {
          console.log('raf');
      
          Promise.resolve().then(function onFulfill2() {
              console.log('promise2');
          });
      });
      
      Promise.resolve().then(function onFulfill1() {
          console.log('promise1');
      });
      
      requestIdleCallback(function onIdle1() {
          console.log('idle1');
      });
      
      setTimeout(function onTimeout() {
          console.log('timeout');
      
          requestIdleCallback(function onIdle2() {
              console.log('idle2');
          });
      }, 0);
      ```
      ```js
      console.log("开始");
      setTimeout(() => {
          console.log("输出一个信息");
      }, 0);
      console.log("执行");
      new Promise((resolve, reject) => {
          console.log("执行for循环");
          for (var i = 0; i < 100; i++) {
              i == 99 && resolve();
          }
          reject();
      })
          .then(() => {
              console.log("执行then函数");
          })
          .catch(() => {
              console.log("catch error");
          });
      console.log("执行结束")
      ```
      - final
        - [promise.then 中 return Promise.resolve 后，发生了什么？ - 徐鹏跃的回答 - 知乎](https://www.zhihu.com/question/453677175/answer/1841325386)
    - this 指向问题
      ```
      var length = 1
      function fn() {
          console.log(this.length);
      }
      var obj = {
          length: 4,
          test: function(t) {
              t()
              arguments[0]()
          }
      }
      obj.test(fn, 6)
      ```
  - css 基础
    - 居中布局（基本）
  - ts
    - infer（加分）
    - 工具类型（如果简历写了，那就是基本，没写就是加分）
    - [什么时候推荐用 type 什么时候用 interface ？](https://pro.ant.design/zh-CN/docs/type-script#%E4%BB%80%E4%B9%88%E6%97%B6%E5%80%99%E6%8E%A8%E8%8D%90%E7%94%A8-type-%E4%BB%80%E4%B9%88%E6%97%B6%E5%80%99%E7%94%A8-interface-)
  - 前端框架
  - 工程化
  - 网络
  - git
  - 实战经验考察
  - 手写功能
- 用人需求（加分） 10min
  - 开源贡献
  - 技术选型
  - svg
    - svg 元素有哪些特有的元素
    - path
      - attr.d
  - canvas
    - 绘图
    - 优化？
  - angular
    - 基本用法
    - rxjs
    - 装饰器
    - 生命周期
- 科班相关（非科班必须）
  - 四大科目
  - linux 基础、命令
    - awk 正则
- 算法 10 min（重点分，速度快加分）
  - 三数之和 （必须，除非项目特别好）
    - 最长递增子序列（非科班必须）
  - 另外再上个难度
- 反问

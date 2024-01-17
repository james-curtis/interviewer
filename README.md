# interviewer
面试官经验

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
      ```js
      setTimeout(function onTimeout() {
        console.log('timeout');
      
        requestIdleCallback(function onIdle2() {
          console.log('idle2');
        });
      }, 0);
      
      Promise.resolve().then(function onFulfill1() {
        console.log('promise1');
      });
      
      requestAnimationFrame(function onAf() {
        console.log('raf');
      
        Promise.resolve().then(function onFulfill2() {
          console.log('promise2');
        });
      });
      
      requestIdleCallback(function onIdle1() {
        console.log('idle1');
      });
      ```
  - css 基础
    - 居中布局
  - ts
    - infer
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
  - canvas
    - 绘图
  - angular
    - 基本用法
    - rxjs
    - 装饰器
    - 生命周期
- 科班相关（非科班必须）
  - 四大科目
- 算法 10 min（重点分，速度快加分）
  - 三数之和 （必须，除非项目特别好）
  - 另外再上个难度
- 反问

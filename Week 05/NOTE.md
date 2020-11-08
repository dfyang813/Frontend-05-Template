学习笔记   
## Proxy   

Proxy 可以对目标对象的读取、函数调用等操作进行拦截，然后进行操作处理。它不直接操作对象，而是像代理模式，通过对象的代理对象进行操作，在进行这些操作时，可以添加一些需要的额外操作。   
### 基本使用   
```
var obj = {
  name: 'tom',
  age: 20,
}
new Proxy(obj, {
  set (obj, prop, val) {

  },
  get (obj, prop){

  }
})
```
第一个参数是目标对象，第二个参数是一个对象，里面包含set方法设置属性值，get方法获取变化属性



## Range   

Range 对象表示文档的连续范围区域.   
创建range对象的方法：document.createRange()   
改变范围的开始点和结束点需要调用方法： setStart()和setEnd()  
通过调用getBoundingClientRect() 方法可以获取到元素的大小及其相对于视口的位置 

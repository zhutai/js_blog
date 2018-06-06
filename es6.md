es6 let 作用域

```js
try{
	if(true){
	var a1 = "a1";
	let a2 = "a2";
	}
	console.log(a1,a2);
}catch(e){
  console.log(e);
}
```
es6字符串

```js
let names = "zhutai",ages = "24";
console.log(`我的名字叫${names}，今年${ages}岁`);
```

es6函数默认赋值，=>后面没有{}括号直接return返回数据
```js
const hello = (name = "zhutai",age = 24) => (
    `我的名字叫${name}，今年${age}岁`
);
console.log(hello("fanming",22));
```

es6 ...直接将数组中的值转换成参数
```
let arr = ["shengming",26];
console.log(hello.apply(null,arr));
console.log(hello(...arr));
```

es6对象的 key value 方法
```
const obj = {name:"zhutai",age:"24"};
const obj1 = {"name1":"shengming",age1:"26"};
console.log(Object.keys(obj));
console.log(Object.values(obj));
```

es6的对象合并
```
const obj3 = {...obj,...obj1,data:"2018"};
console.log(obj3);
```

es6的数据解构   数组和对象
```
let [arrname,arrage] = arr;
console.log(arrname,"|",arrage);
const {name,age} = obj;
console.log(name,"|",age);
```

es6 class 类
```
class Box{
	constructor(name){
     	this.name = name || "zhutai";
	}
	getName(){
		console.log(`这个值是${this.name}`);
	}
}

const App = new Box("china");
App.getName();
```


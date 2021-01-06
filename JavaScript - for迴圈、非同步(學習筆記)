# JavaScript - for迴圈、非同步(學習筆記)

## if/else
statement(敘述式):沒有回傳值
expression(判斷式):可以被印出來（console.log）
```
let x = 1;
let y = 2;
if(z = x + y){

}
```
## for...loop
```
for(let X = 0; x < array.length; x++){
    const a = array[x];
}
```
## for...in
#### 迭代key
```
for (const key in foo ){
    console.log(key)
}
for (const key in foo){

}
```
## for...of
#### iterate 迭代器
```
    for (const value of Object.values(bar){
        console.log(value)
    }
```
## React 單一原則(盡量用immutable)
### mutabale 可變
```
const foo = ['a','b','c']
const bar = {a: 1,b: 2,c: 3}

bar.a = 2
console.log(bar)
```
### immutable 不可變
```
    console.log(
    "spread",
        {
            //spread syntax
            ...bar,
            a: 2
        }   
    )
    console.log("bar",bar)
```
### spread語法：（["first", ...array, "last"]）
ES6中資料會因前後順序被覆蓋
含頭不含尾
```
array.slice（0,2）取得0往後2個位置的value

const foo = ["a", "b", "c", "d", "e"];

//移除index位置的value

let index = 3;
const foo1 = [
  //spread syntax
  //串接2串slice
  ...foo.slice(0, index),
  ...foo.slice(index + 1)
];
console.log(foo1);
```
## 解構語法 destruction
```
    const foo = ['a','b','c']
    const bar = {
        a: 1,
        b: 2,
        c: 3
    }
    
    const{ a , ...rest } = bar
    console.log("rest",rest)
    
    const[x , y, ...rest] = foo
    console.log)(x , y, rest2)
```
# function
```
//argument 引數
//parameter 參數

function(arg1, arg2){
    return arg1 + arg2
}
console.log(foo(1,2))
```
### arrow function(ES6)
```
const foo = (arg1, arg2) =>{
return arg1 + arg2
}
```
### setTimeout(延遲處理)
```
setTimeout(
    () => {
    console.log('in setTimeout')
    },
    1000
)
```
### promise(expresstion)
寫出來立即執行，可用函式包住
使用.then .catch
**getMYPromise
```
const myPromise = new Promise((resolove, reject) => {
    const x= 1
    if (x>0){
        resolve(x)
    } else {
        reject("qq")
    }
})

myPromise

.then((data) => {
    return data + 1
})
//沒問題進入then
.then((data) => {
    return data + 2
})
//出問題進入catch
.catch((error) => {
    
})

```
### async(非同步) / await（等待）
async function：回傳promise的簡寫
防止函式暴掉可使用try...catch
```
const getMYNewPromise = async (a, b) =>{
    
    try{
        const user = await getUser()
    }catch(error){
    
    }


    const x = a+ b 
    if(x > 0){
        return x
    } else {
    throw new Error('qq')
    }
}

```
### 不使用promise跟async的情況下，可使用callback function（回調）
```
//callback = bar的callback function

const bar = (callback) =>{
    callback()
}
////

const bar = (a, b, sussessCallback, failtureCallback) =>{
    const x = a + b
    
}
bar(() =>{
    console.log('i am callback')
})
```

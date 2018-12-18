# Shared by huli
1. 請描述一下 cookies, sessionStorage 和 localStorage 的區別？
2. 如何實現瀏覽器內多個標籤頁之間的通信？
3. css 隱藏元素的幾種方法 （至少寫出三種）
4. css 置中 （包括水平置中和垂直置中）
5. css3 中的 transform 屬性和 transition 屬性？
6. JS apply 和 call 的用法和區別？
7. 針對 jQuery 的優化方法？
8. jQuery.extend 與 jQuery.fn.extend 的區別？
9. 請講述前端跨域問題產生及解決方法？
10. 請輸入以下代碼輸出的是什麼？為什麼？

```var a = 1;
function fn(){
  console.log(a);
  var a = 5;
  console.log(a);
  a++;
  var a;
  fn2();
  console.log(a);
  function fn2(){
    console.log(a);
    a = 20;
    b = 100;
  }
}
fn();
console.log(a);
a = 10;
console.log(a);
console.log(b);```

# Shared by Lin 
1. inline elements 和 block-level elements 各有哪些？差異為何？
  如何轉換 block-level elements 為 inline elements？
  inline elements 的 padding 和 margin 可設置嗎？
2. 請描述幾種 css 水平置中和垂直置中的方式。
3. 請描述 css3 和 html5 新特性。
4. 請列舉前端性能優化的方法。
5. 請舉例描述 es6 新的特性另請解釋 promise。
6. 請寫出下面 js 的輸出
 ```6-1
  for(var i=1; i<5; i++){
    setTimeout(function() {
      console.log(i);
    }, i * 1000);
  }
  6-2
  function test() {
    console.log(a);
    console.log(foo());
    var a = 1;
    function foo() {
      return 2;
    }
  }
  test();
  6-3
  var f = true;
  if(f === true) {
    var a =10;
  }
  function fn() {
    var b = 20;
    c = 30
  }
  fn();
  console.log(a, b, c);
  6-4
  var a = [1, 2, 3];
  var b = a;
  a.push(5);
  var obj = { 1: 'a', 2: b};
  console.log(b, obj[0], obj[1], obg.2);
  6-5
  var fullname = 'John Doe';
  var obj = {
    fullname: 'Colin Ihrig',
    prop: {
      fullname: 'Aurelio De Rosa',
      getFullname: function() {
        return this.fullname;
      }
    }
  };
  console.log(obj.prop.getFullname());
  var test = obj.prop.getFullname;
  console.log(test());
  6-6
  請用 JS 寫出能計算婓波那契數列（Fibonacci）第 N 個值的函式。
  (0, 1, 1, 2, 3, 5, 8, 13, 21...)```
  
# Shared by Marin
面試經驗分享（一）
公司 : 惠訊國際股份有限公司
職缺 : java 軟體工程師
大致內容 :
沒有筆試，到公司後填寫基本資料直接開始面試，同時有兩位主管進行面試。
先是自我介紹，因為我只提了前一份工作的內容，所以後續問題也都圍繞在上面。

問題大概是：
1. 工作用了哪些技術及框架？
2. 工作的時候有遇上什麼問題及你怎麼解決的？
3. 為什麼要離職？
4. 透過哪些管道學習新技術的？書籍？還是網路？
5. 離職至今的待業期你做了哪些事情？
6. 聽過 JavaScript 的 Hoisting 嗎？

以我還記得的差不多就這些……
然後就是邊介紹進公司的工作內容，邊進行提問，一些比較私人的問題我就略過了，諸如像是通勤、薪資等的。

我個人有提出的問題是：
1. 每周/每日的工作流程是什麼？
2. 除了我之外大概還有幾位同職級的人員？

然後就差不多告一個段落了。
面試包含填資料的總花費時間大概是 50 分鐘。
雖然是職稱是掛 java 軟體工程師，但其實比較偏全端吧，因為網頁那塊也是要去負責。
我後續還有幾間面試，也會盡可能把還記得的部分跟大家說。
至於我的回答因為每個人的想法都不太一樣，所以我就不提供了，有興趣可以私訊討論。
不知道這類型的分享對各位有沒有幫助，如果有什麼想知道的就提出來沒關係，我可以就我知道的再補充。 

# Shared by huli
1. 為什麼要初始化 CSS 樣式？
2. 請問如何使用 JavaScript 選取此 DOM `<div class='menu'></div>`
3. 請排出 CSS 優先層級：!importent、tag、id、class。
4. 要寫一個支援 RWD 的網頁，主要使用 CSS 哪個語法？
5. 若不用 float 要如何讓 div 並排？
### 請寫出下列程式 console.log 結果：

```js
var oneadAry = ['a', 'b', 'c'];
oneadAry.push('b');
console.log(oneadAry);

oneadAry.pop();
console.log(oneadAry);

oneadAry.shift();
console.log(oneadAry);

oneadAry.unshift('d');
console.log(oneadAry);

var tempAry = oneadAry.slice(0, 2);
console.log(tempAry);
```

- 請用 foreach 列出 oneadAry 所有值。

### 請用 prototype 講 `oneadObj` 加入一個 `name` 屬性，並給值為你的英文名字。

### 以下程式碼 `console.log` 的結果是：

```js
var foo = 'Hello';
(function() {
  var bar = ' World';
  console.log(foo + bar);
})();
console.log(foo + bar);
```

### 試寫出 json 資料格式。

### 試寫出 JavaScript 如何接收 jsonp。

### `'=='` 和 `'==='` 有什麼不同？

### 以下程式改用三元運算式寫法：

```js
if (oneadAry.length == 0) {
  console.log('true');
} else {
  console.log('false');
}
```

### 以下程式兩個判斷式各為什麼結果？

```js
var onead;
if(onead === undefined) {
  console.log('true');
} else {
  console.log('false');
}

if (onead === 'undifined') {
  console.log('true');
} else {
  console.log('false');
}
```

### 給定一個圖片網址，在拿到圖片後將圖片的寬高設定為 640px、360px，寫出三種作法（Promise 是其中一個）。

```js
var imgUrl = 'http://someimages.com/i.png';
```

### 請用 Singleton 方式實作出一個 `oneadObj` 物件。

### 請用 Factory Design Pattern 方式實作一個 `oneadObj` 物件。

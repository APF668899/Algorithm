# 大O表示法
## 时间复杂度(代码执行的时间)
```js
for(var i = 1;i <= n ;i++){
	x++
}
```
时间复杂度:O(1+3n) = O(n)
```js
for(var i = 1;i <= n;i++){
	for(var j = 1;i <= m;j++){
	x++;
	}	
}
```
时间复杂度:O(mn)
```js
for(var i = 1;i <= n ;i++){
	x++
}
for(var i = 1;i <= n;i++){
	for(var j = 1;i <= m;j++){
	x++;
	}	
}
```
时间复杂度:O(n + n<sup>2</sup>) = O(n<sup>2</sup>)
常见的时间复杂度量级(从低到高)
* 常数阶O(1)
  ```js
	var a = 0;
	var b = 1;
	var c = a;
	a = b;
	b = c;
  ```

* 对数阶O(logN)
  ```js
  var i= 1;
  while(i < n){
	  i = i * 2;
  }
  ```
  * 2<sup>k</sup> = n
  * 次数:k = log<sup>N</sup> 
* 线性阶O(n)
  ```js
		for(var i = 1;i <= n ;i++){
			x++
		}
	```
* 线性对数阶O(nlogN)
	```js
		for(var i = 1;i <= n ;i++){
			int x = 1;
			while(x < n){
				x = x * 2;
			}
		}
	```   
* 平方阶O(n<sup>2</sup>)
  ```js
	   for(var i = 1;i <= n;i++){
		    for(var j = 1;i <= n;j++){
		       x++;
		   }	
		}
  ```
* 立方阶O(n<sup>3</sup>)
* K次阶O(n<sup>k</sup>)
* 指数阶(2<sup>n</sup>)
* 阶乘O(n!)
## 空间复杂度:内存空间增长的趋势
* O(1)
   ```js
	   var x = 0;
	   var y = 0;
	   x++;
	   y++
	```   
* O(N)
  ```js
  var array = [];
  for(var i = 0;i < n;i++){
	  array[i] = i;
  }
  ```
* O(N<sup>2</sup>)
  ```js
  var array = [][];
  for(var i = 0;i < n;i++){
	  for(var j = 0;j < n ;j++){
		  array[i][j] = i;
	  }
  }
  ```

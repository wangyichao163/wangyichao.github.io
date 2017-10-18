## 1、取二维数组中最大值的几种方法

```js

		function largestOfFour(arr){
			//将二维数组中的最大数放到数组中
			let resultArr = [];
			//遍历二维数组的外层
			for(let i=0;i<arr.length;i++){
				//创建一个变量来存储最大数
				let bigNum = 0;
				//遍历二维数组的内层
				for(let j=0;j<arr[i].length;j++){
					//判断最大数和二维数组中数字大小
					if(arr[i][j] > bigNum){
						//给最大数变量赋值
						bigNum = arr[i][j];
					}
				}
				resultArr[i] = bigNum;
			}
			return resultArr;
		}

```

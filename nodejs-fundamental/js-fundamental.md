# I.Javascript Fundamental

## 1.Javascript là gì?

-   JavaScript là một ngôn ngữ lập trình thông dịch (interpreted programming language) được sử dụng phổ biến trong phát triển web.

-   JavaScript được sử dụng để thêm các tính năng tương tác cho các trang web.

-   JavaScript có thể được nhúng vào trong các trang web thông qua thẻ `<script>`.

-   JavaScript có thể được sử dụng để viết các ứng dụng web, ứng dụng desktop, ứng dụng di động, ứng dụng máy chủ, ứng dụng trò chơi, ... .

## 2.Các tính năng của Javascript

-   JavaScript là một ngôn ngữ lập trình động (dynamic programming language) có thể thực thi trực tiếp trên trình duyệt mà không cần biên dịch.

-   JavaScript là một ngôn ngữ lập trình hướng đối tượng (object-oriented programming language).

-   JavaScript là một ngôn ngữ lập trình hướng sự kiện (event-driven programming language).

-   JavaScript là một ngôn ngữ lập trình bất đồng bộ (asynchronous programming language).

-   JavaScript là một ngôn ngữ lập trình đa nền tảng (cross-platform programming language).

-   JavaScript là một ngôn ngữ lập trình dễ học (easy to learn programming language).

## 3. Kiến thức cần có

### 3.1 Variables and data types

#### a. Biến(Variables):

-   Dùng để lưu trữ dữ liệu
-   Sử dụng từ khóa **var**, **let** và **const**
-   Ví dụ:

```js
var myVariable = 10
let anotherVariable = 'Hello'
const pi = 3.14
```

#### b. Kiểu dữ liệu(Data types):

-   Các kiểu dữ liệu cơ bản trong JavaScript bao gồm: Number, String, Boolean, Object, Array, Null, Undefined.
-   Sử dụng typeof để kiểm tra kiểu dữ liệu của một biến.
-   Ví dụ:

```js
var numberVar = 42
var stringVar = 'Hello, World!'
var booleanVar = true
var objectVar = { key: 'value' }
var arrayVar = [1, 2, 3]
var nullVar = null
var undefinedVar

console.log(typeof numberVar) // "number"
```

###### Kiểu dữ liệu số (Number):

-   JavaScript sử dụng kiểu dữ liệu số để đại diện cho cả số nguyên và số thực.
    -Có thể thực hiện các phép toán cơ bản như cộng, trừ, nhân, chia.
    -Ví dụ:

```js
var integerNumber = 42
var floatNumber = 3.14

console.log(integerNumber + floatNumber) // 45.14
```

###### Kiểu Dữ Liệu Chuỗi (String):

**Khai Báo và Sử Dụng Chuỗi:**

-   Chuỗi là một dãy các ký tự.
-   Có thể sử dụng dấu nháy đơn hoặc dấu nháy kép để khai báo chuỗi.

**Phương Thức Chuỗi:**

-   Sử dụng các phương thức như length, charAt, substring để làm việc với chuỗi.
-   Ví dụ:

```js
var myString = 'Hello, World!'
console.log(myString.length) // 13
console.log(myString.charAt(0)) // "H"
console.log(myString.substring(0, 5)) // "Hello"
```

###### Kiểu Dữ Liệu Boolean:

-   Biểu diễn giá trị đúng (true) hoặc sai (false).
-   Thường được sử dụng trong các điều kiện và câu lệnh điều kiện.

###### Kiểu Dữ Liệu Đối Tượng (Object):

-   Đối tượng là một tập hợp các thuộc tính (properties) và phương thức (methods).
-   Ví dụ:

```js
var person = {
	name: 'John',
	age: 30,
	isStudent: false,
	sayHello: function () {
		console.log('Hello!')
	},
}

console.log(person.name) // "John"
person.sayHello() // "Hello!"
```

##### Kiểu Dữ Liệu Mảng (Array):

-   Mảng là một tập hợp các giá trị.
-   Sử dụng chỉ số để truy xuất và thay đổi giá trị trong mảng.
-   Kiểu dữ liệu của các giá trị trong mảng có thể giống hoặc khác nhau
-   Ví dụ:

```js
var numbers = [1, 2, 3, 4, 5]
var fruits = ['apple', 'banana', 'orange']
var a = [
	1,
	'b',
	{
		name: 'join',
	},
	true,
]

console.log(numbers[2]) // 3
console.log(fruits.length) // 3
```

###### Kiểu Dữ Liệu Null và Undefined:

-   **null** đại diện cho giá trị không tồn tại hoặc không biết.
-   **undefined** đại diện cho biến chưa được gán giá trị.

###### Ép Kiểu Dữ Liệu (Type Conversion):

-   JavaScript có thể tự động ép kiểu dữ liệu.
-   Sử dụng các hàm như Number(), String(), Boolean() để ép kiểu rõ ràng.
-   Ví dụ:

```js
var x = '5'
var y = 10

console.log(x + y) // "510"
console.log(Number(x) + y) // 15
```

### 3.2 Toán tử (Operators)

#### a. Toán tử số học (Arithmetic operators):

-   Các toán tử số học bao gồm: cộng (+), trừ (-), nhân (\*), chia (/), chia lấy dư (%), tăng (++), giảm (--).

```js
var x = 10
var y = 3

console.log(x + y) // 13

console.log(x - y) // 7

console.log(x * y) // 30

console.log(x / y) // 3.3333333333333335

console.log(x % y) // 1

console.log(x++) // 10

console.log(x--) // 11
```

#### b. Toán tử gán (Assignment operators):

-   Các toán tử gán bao gồm: (=), (+=), (-=), (\*=), (/=), (%=).

```js
var x = 10
x += 5 // x = x + 5

console.log(x) // 15
```

#### c. Toán tử so sánh (Comparison operators):

-   Các toán tử so sánh bao gồm: (==), (!=), (>), (<), (>=), (<=).

```js
var x = 10
var y = 3

console.log(x == y) // false

console.log(x != y) // true

console.log(x > y) // true

console.log(x < y) // false

console.log(x >= y) // true

console.log(x <= y) // false
```

#### d. Toán tử logic (Logical operators):

-   Các toán tử logic bao gồm: (&&), (||), (!).

```js
var x = 10
var y = 3

console.log(x > 5 && y < 10) // true

console.log(x > 5 || y > 10) // true

console.log(!(x > 5)) // false
```

#### e. Toán tử chuỗi (String operators):

-   Toán tử (+) có thể được sử dụng để nối chuỗi.

```js
var firstName = 'John'
var lastName = 'Doe'

console.log(firstName + ' ' + lastName) // "John Doe"
```

#### f. Toán tử điều kiện (Conditional operators):

-   Toán tử điều kiện (?:) có thể được sử dụng để thay thế cho câu lệnh if.

```js
var age = 20

var result = age >= 18 ? 'Adult' : 'Child'

console.log(result) // "Adult"
```

#### g. Toán tử typeof:

-   Toán tử typeof có thể được sử dụng để kiểm tra kiểu dữ liệu của một biến.

```js
var x = 10

console.log(typeof x) // "number"
```

#### h. Toán tử in:

-   Toán tử in có thể được sử dụng để kiểm tra một thuộc tính có tồn tại trong một đối tượng hay không.

```js
var person = {
	name: 'John',
	age: 20,
}

console.log('name' in person) // true

console.log('address' in person) // false
```

#### i. Toán tử instanceof:

-   Toán tử instanceof có thể được sử dụng để kiểm tra một đối tượng có phải là một thể hiện của một lớp hay không.

```js
var person = {
	name: 'John',
	age: 20,
}

console.log(person instanceof Object) // true
```

#### k. Toán tử ba ngôi (Ternary operator):

-   Toán tử ba ngôi có thể được sử dụng để thay thế cho câu lệnh if.

```js
var age = 20

var result = age >= 18 ? 'Adult' : 'Child'

console.log(result) // "Adult"
```

### 3.3 Mảng (Arrays)

#### a. Khai báo mảng (Array literals):

-   Cú pháp:

```js
var arrayName = [item1, item2, item3]
```

-   Ví dụ:

```js
var numbers = [1, 2, 3, 4, 5]

var fruits = ['Apple', 'Banana', 'Orange']
```

#### b. Truy xuất phần tử (Accessing array elements):

-   Cú pháp:

```js
arrayName[index]
```

-   Ví dụ:

```js
var numbers = [1, 2, 3, 4, 5]

console.log(numbers[0]) // 1

console.log(numbers[1]) // 2

console.log(numbers[2]) // 3

console.log(numbers[3]) // 4

console.log(numbers[4]) // 5
```

#### c. Thay đổi phần tử (Modifying array elements):

-   Cú pháp:

```js
arrayName[index] = newValue
```

-   Ví dụ:

```js
var numbers = [1, 2, 3, 4, 5]

numbers[0] = 10

console.log(numbers) // [10, 2, 3, 4, 5]
```

#### d. Độ dài mảng (Array length):

-   Cú pháp:

```js
arrayName.length
```

-   Ví dụ:

```js
var numbers = [1, 2, 3, 4, 5]

console.log(numbers.length) // 5
```

#### e. Phương thức mảng (Array methods):

-   Các phương thức mảng bao gồm: push, pop, shift, unshift, splice, slice, concat, join, indexOf, lastIndexOf, includes, reverse, sort, forEach, map, filter, reduce.

##### f. Phương thức push:

-   Cú pháp:

```js

arrayName.push(item1, item2, ...)
```

-   Ví dụ:

```js
var numbers = [1, 2, 3, 4, 5]

numbers.push(6, 7)

console.log(numbers) // [1, 2, 3, 4, 5, 6, 7]
```

### 3.4 Câu lệnh (Statements)

#### a. Câu lệnh điều kiện (Conditional statements):

-   Câu lệnh if:

```js
var age = 20

if (age >= 18) {
	console.log('Adult')
} else {
	console.log('Child')
}
```

-   Câu lệnh switch:

```js
var day = 2

switch (day) {
	case 0:
		console.log('Sunday')
		break
	case 1:
		console.log('Monday')
		break
	case 2:
		console.log('Tuesday')
		break
	case 3:
		console.log('Wednesday')
		break
	case 4:
		console.log('Thursday')
		break
	case 5:
		console.log('Friday')
		break
	case 6:
		console.log('Saturday')
		break
	default:
		console.log('Invalid day')
}
```

#### b. Câu lệnh lặp (Loop statements):

-   Câu lệnh for:

```js
for (var i = 0; i < 10; i++) {
	console.log(i)
}
```

-   Câu lệnh while:

```js
var i = 0

while (i < 10) {
	console.log(i)
	i++
}
```

-   Câu lệnh do...while:

```js
var i = 0

do {
	console.log(i)
	i++
} while (i < 10)
```

### 3.5 Hàm (Functions)

#### a. Khai báo hàm (Function declarations):

-   Cú pháp:

```js
function functionName(parameter1, parameter2, parameter3) {
	// code block
}
```

-   Ví dụ:

```js
function sum(a, b) {
	return a + b
}

console.log(sum(1, 2)) // 3
```

**Ghi chú:** Hàm có thể được khai báo bên trong một hàm khác.

```js
function sum(a, b) {
	function double(x) {
		return x * 2
	}

	return double(a) + double(b)
}

console.log(sum(1, 2)) // 6

console.log(double(1)) // ReferenceError: double is not defined
```

**Arrow function:**

-   Dùng để viết hàm ngắn gọn hơn.

-   Được giới thiệu trong ES6.

-   Cú pháp:

```js
;(parameter1, parameter2, parameter3) => {
	// code block
}
```

-   Ví dụ:

```js
var sum = (a, b) => {
	return a + b
}

console.log(sum(1, 2)) // 3
```

-   Nếu hàm chỉ có một câu lệnh return thì có thể viết ngắn gọn như sau:

```js
var sum = (a, b) => a + b

console.log(sum(1, 2)) // 3
```

-   Nếu hàm chỉ có một tham số thì có thể bỏ dấu ngoặc đơn:

```js
var double = (x) => x * 2

console.log(double(1)) // 2
```

-   Nếu hàm không có tham số thì phải sử dụng dấu ngoặc đơn:

```js
var sayHello = () => console.log('Hello, World!')

sayHello() // "Hello, World!"
```

-   Nếu hàm trả về một đối tượng (hoặc mảng) thì phải sử dụng dấu ngoặc đơn:

```js
var createPerson = () => ({ name: 'John', age: 20 })

console.log(createPerson()) // { name: "John", age: 20 }
```

#### b. Biểu thức hàm (Function expressions):

-   Cú pháp:

```js
var functionName = function (parameter1, parameter2, parameter3) {
	// code block
}
```

-   Ví dụ:

```js
var sum = function (a, b) {
	return a + b
}

console.log(sum(1, 2)) // 3
```

#### c. Hàm ngay lập tức (Immediately invoked function expressions):

-   Cú pháp:

```js
;(function () {
	// code block
})()
```

-   Ví dụ:

```js
;(function () {
	console.log('Hello, World!')
})() // "Hello, World!"
```

#### d. Hàm có tham số mặc định (Default parameters):

-   Cú pháp:

```js
function functionName(parameter1 = defaultValue1, parameter2 = defaultValue2) {
	// code block
}
```

-   Ví dụ:

```js
function sum(a = 0, b = 0) {
	return a + b
}

console.log(sum(1)) // 1
```

#### f. Hàm có tham số rest (Rest parameters):

-   Cú pháp:

```js
function functionName(...restParameters) {
	// code block
}
```

-   Ví dụ:

```js
function sum(...numbers) {
	var result = 0

	for (var number of numbers) {
		result += number
	}

	return result
}

console.log(sum(1, 2, 3, 4, 5)) // 15
```

#### g. Hàm có tham số spread (Spread parameters):

-   Cú pháp:

```js
function functionName(parameter1, parameter2, ...spreadParameters) {
	// code block
}
```

-   Ví dụ:

```js
function sum(a, b, ...numbers) {
	var result = a + b

	for (var number of numbers) {
		result += number
	}

	return result
}

console.log(sum(1, 2, 3, 4, 5)) // 15
```

## 4. Callback và Bất đồng bộ trong Javascript (Callback and Asynchronous in Javascript)

### 4.1 Callback

#### a. Định nghĩa

-   Callback là một hàm được truyền qua đối số và được gọi lại trong hàm khác.

-   Callback được sử dụng để đảm bảo rằng một đoạn code chỉ được thực thi sau khi một đoạn code khác đã thực thi xong.

#### b. Ví dụ

-   Ví dụ 1:

```js
function doSomething(callback) {
	console.log('do something')

	callback()
}

function sayHello() {
	console.log('Hello, World!')
}

doSomething(sayHello) // "do something" "Hello, World!"
```

#### c. Callback hell

-   Callback hell là một tình huống xảy ra khi một hàm callback được gọi bên trong một hàm callback khác.

-   Ví dụ:

```js
function doSomething(callback) {
	console.log('do something')

	callback()
}

function doSomethingElse(callback) {
	console.log('do something else')

	callback()
}

function end() {
	console.log('end')
}

doSomething(function () {
	doSomethingElse(function () {
		end()
	})
}) // "do something" "do something else" "end"
```

==> Có thể thấy rằng khi sử dụng callback hell thì mã nguồn sẽ trở nên khó đọc và khó bảo trì.

### 4.2 Bất đồng bộ (Asynchronous)

#### a. Định nghĩa

-   Bất đồng bộ là một phương thức thực thi một tác vụ mà không phải chờ tác vụ trước đó thực thi xong.

-   Bất đồng bộ được sử dụng để đảm bảo rằng một đoạn code chỉ được thực thi sau khi một đoạn code khác đã thực thi xong.

#### b. Ví dụ

-   Ví dụ 1:

```js
function doSomething() {
	console.log('do something')
}

function doSomethingElse() {
	console.log('do something else')
}

function end() {
	console.log('end')
}

setTimeout(function () {
	doSomething()

	setTimeout(function () {
		doSomethingElse()

		setTimeout(function () {
			end()
		}, 1000)
	}, 1000)
}, 1000) // "do something" "do something else" "end"
```

==> Có thể thấy rằng khi sử dụng bất đồng bộ thì mã nguồn sẽ trở nên khó đọc và khó bảo trì.

#### c. Promise

##### i. Định nghĩa

-   Promise là một đối tượng đại diện cho một giá trị chưa được xác định tại thời điểm hiện tại nhưng có thể được xác định tại một thời điểm trong tương lai.

-   Promise được sử dụng để thay thế cho callback và giải quyết được vấn đề callback hell.

##### ii. Cú pháp khai báo và sử dụng

-   Cú pháp khai báo:

```js
var promise = new Promise(function (resolve, reject) {
	// code block
})
```

-   Cú pháp sử dụng:

```js
promise
	.then(function (value) {
		// code block
	})
	.catch(function (error) {
		// code block
	})
	.finally(function () {
		// code block
	})
```

-   Giải thích:

    -   Hàm khởi tạo của **Promise** nhận vào một hàm với hai tham số là **resolve** và **reject**.
    -   Hàm **resolve** được gọi khi một giá trị được xác định.
    -   Hàm **reject** được gọi khi một giá trị không được xác định.
    -   Phương thức **then** được sử dụng để thực thi một đoạn code khi một giá trị được xác định.
    -   Phương thức **catch** được sử dụng để thực thi một đoạn code khi một giá trị không được xác định.
    -   Phương thức **finally** được sử dụng để thực thi một đoạn code khi một giá trị được xác định hoặc không được xác định.

-   Ví dụ:

```js
var promise = new Promise(function (resolve, reject) {
	setTimeout(function () {
		resolve('success')
	}, 1000)
})

promise.then(function (value) {
	console.log(value) // "success"
})
```

##### iii. Phương thức Promise.all()

-   Phương thức Promise.all() được sử dụng để chờ cho tất cả các promise được truyền vào được giải quyết.

-   Cú pháp:

```js

Promise.all([promise1, promise2, ...]).then(function(values) {
  // code block
})
```

-   Ví dụ:

```js
var promise1 = new Promise(function (resolve, reject) {
	setTimeout(function () {
		resolve('promise 1')
	}, 1000)
})

var promise2 = new Promise(function (resolve, reject) {
	setTimeout(function () {
		resolve('promise 2')
	}, 2000)
})

Promise.all([promise1, promise2]).then(function (values) {
	console.log(values) // ["promise 1", "promise 2"]
})
```

#### d. Async/Await

##### i. Định nghĩa

-   Async/Await là một cú pháp được sử dụng để viết bất đồng bộ một cách đồng bộ.

-   Async/Await được sử dụng để thay thế cho Promise.

##### ii. Cú pháp khai báo và sử dụng

-   Cú pháp khai báo:

```js
async function functionName() {
	// code block
}
```

-   Cú pháp sử dụng:

```js
async function functionName() {
	var value = await promise

	// code block
}
```

-   Giải thích:

    -   Hàm khai báo **async** được sử dụng để khai báo một hàm bất đồng bộ.
    -   Từ khóa **await** được sử dụng để chờ cho một promise được giải quyết.
    -   Khi một promise được giải quyết thì giá trị của promise đó được gán cho biến được khai báo bên trên từ khóa **await**.
    -   Khi một promise được giải quyết thì đoạn code bên dưới từ khóa **await** được thực thi.

-   Ví dụ:

```js
async function doSomething() {
	var promise = new Promise(function (resolve, reject) {
		setTimeout(function () {
			resolve('success')
		}, 1000)
	})

	var result = await promise

	console.log(result) // "success"
}

doSomething()
```

##### iii. Ví dụ về việc sử dụng Async/Await thay thế cho Promise

-   Ví dụ 1:

```js
function doSomething() {
	return new Promise(function (resolve, reject) {
		setTimeout(function () {
			resolve('success')
		}, 1000)
	})
}

function doSomethingElse() {
	return new Promise(function (resolve, reject) {
		setTimeout(function () {
			resolve('success')
		}, 1000)
	})
}

function end() {
	console.log('end')
}

doSomething()
	.then(function () {
		return doSomethingElse()
	})
	.then(function () {
		end()
	})
```

==> Có thể thấy rằng khi sử dụng Promise thì mã nguồn sẽ trở nên khó đọc và khó bảo trì.

```js
async function doSomething() {
	await doSomething()

	await doSomethingElse()

	end()
}
```

==> Có thể thấy rằng khi sử dụng Async/Await thì mã nguồn sẽ trở nên dễ đọc và dễ bảo trì.

# II. Bài tập

## 1. Bài tập 1

-   Viết chương trình nhập vào một số nguyên dương n và tính tổng các ước số nhỏ hơn chính nó.

-   Ví dụ:

```js
Input: 10

Output: 8(1 + 2 + 5)
```

## 2. Bài tập 2

-   Viết chương trình nhập vào một số và tỉnh tổng các chữ số của số đó.

-   Ví dụ:

```js
Input: 123

Output: 6(1 + 2 + 3)
```

## 3. Bài tập 3

-   Viết chương trình nhập vào một mảng các số nguyên và tính tổng các số chẵn trong mảng đó.

-   Ví dụ:

```js
Input: [1, 2, 3, 4, 5]

Output: 6(2 + 4)
```

## 4. Bài tập 4

-   Viết chương trình nhập vào một mảng các số nguyên và tính tổng các số nguyên tố trong mảng đó.

-   Ví dụ:

```js
Input: [1, 2, 3, 4, 5]

Output: 5(2 + 3)
```

**Gợi ý:** Số nguyên tố là số chỉ chia hết cho 1 và chính nó.

### Lưu ý:

-   Các bài tập trên là các bài tập cơ bản để kiểm tra kiến thức cơ bản về Javascript.

-   Các bài tập trên có thể giải quyết được bằng nhiều cách khác nhau.

-   Làm bài tập vào file `js-fundamental.js` và đặt trong thư mục `nodejs-fundamental`.

-   Tạo branch `practice` trên github và push code lên branch đó. (Không push code lên branch `master`, xem trong phần [Git Fundamental](#git-fundamental))

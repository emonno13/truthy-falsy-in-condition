# truthy-falsy-in-condition
Kiểm tra tính đúng đắn ở một câu lệnh điều kiện


**Hướng giải bài 5**
```
// Nhập vào x từ bàn phím

let x = prompt('Nhập vào đi: ')

// Kiểm tra x có phải số hay chuỗi

if (!Number(x)) {
	console.log('Đây là chuỗi')
	console.log('Error')
} else {
	console.log('Đây là số đúng rồi !!!')
	console.log('Bắt đầu thực hiện các phép tính, các câu lệnh điều kiện ghi ở đây ...')
	//..................
}
```

- Okk bình thường khi viết câu lệnh điều kiện thì với những bạn mới học sẽ nghĩ viết if ( x > gì đó ) hoặc if (x < gì đó), ... nghĩa là phải có một biểu thức so sánh bên trong ngoặc if ( )
- Vậy sao bài 5 hướng giải lại là if (!Number(x)).Thế Number(x) hay !Number(x) là gì ???
- Về bản chất là mình đang kiểm tra tính đúng đắn của dieuKien trong if (dieuKien) 
- Giải thích sơ:
  - Nếu nhập vào 1 chuỗi '12 sài gòn' chẳng hạn,thì Number('12 sài gòn') trả về giá trị là NaN ( mang tính chất falsy ).Vậy !Number('12 sài gòn') trả về true ( mang tính chất truthy ).
  #### &rarr; Vậy nếu x = '12 sài gòn ' thì if(!Number(x)) sẽ trở thành mệnh đề đúng ( truthy ), thực thi code ngay bên dưới. 
  ![image](https://user-images.githubusercontent.com/53046415/88463435-f5c9ee00-cedc-11ea-9d8f-9ab7ca5959a3.png)
  #### &rarr; Vậy nếu x = '12' thì if(!Number(x)) sẽ trở thành mệnh đề sai ( falsy ), ko thực thi code bên dưới mà nhảy xuống điều kiện kế tiếp. Ngược lại với cái trên.
  



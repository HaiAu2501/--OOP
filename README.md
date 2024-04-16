# Lập trình hướng đối tượng với Java

## Mục lục

<ol>

<details>

<summary>Phần 1: Giới thiệu</summary>

<li>1. [**Introduction**](1.%20Introduction/)</li>

    1. [HelloWorld](1.%20Introduction/HelloWorld.java)
    2. [HelloJava](1.%20Introduction/HelloJava.java)
    3. [DataTypes](1.%20Introduction/DataTypes.java)
    4. [Wrappers](1.%20Introduction/Wrappers.java)
    5. [Boxing](1.%20Introduction/Boxing.java)
    6. [Arrays](1.%20Introduction/Arrays.java)
    7. [ArgumentPassing](1.%20Introduction/ArgumentPassing.java)
    8. [MethodOverloading](1.%20Introduction/MethodOverloading.java)
    9. [ObjectInJava](1.%20Introduction/ObjectsInJava.java)
    10. [ObjectCreation](1.%20Introduction/ObjectCreation.java)
    11. [ObjectDestruction](1.%20Introduction/ObjectDestruction.java)
    12. [ThisReference](1.%20Introduction/ThisReference.java)

</details>

<details>

<summary>Phần 2: Nguyên lý lập trình hướng đối tượng</summary>

<li>2. [**Object-oriented Programming Principles**](2.%20Object-oriented%20Programming%20Principles/)</li>

    1. [Subclass](2.%20Object-oriented%20Programming%20Principles/Subclass.java)

</details>

<details>

<summary>Phần 3: Cấu trúc dữ liệu và thuật toán</summary>

<li>3. [**Data Structures and Algorithms**](3.%20Data%20Structures%20and%20Algorithms/)</li>

</details>

</ol>

## Máy ảo Java (Java Virtual Machine - JVM)

Java vừa là ngôn ngữ lập trình vừa được **biên dịch** (complied) vừa được **thông dịch** (interpreted). Mã nguồn Java được chuyển thành các lệnh nhị phân đơn giản, giống như mã máy của vi xử lý thông thường. Tuy nhiên, trong khi mã nguồn C hoặc C++ được biến đổi thành các lệnh bản địa cho một mô hình vi xử lý cụ thể, mã nguồn Java được biên dịch thành một định dạng chung - các lệnh cho một máy ảo.

Bytecode Java được thực thi bởi JVM, một máy ảo tiêu chuẩn hóa hoạt động như một bộ xử lý giả lập. JVM giúp Java có khả năng chạy được trên nhiều nền tảng khác nhau mà không cần sửa đổi mã - tính *viết một lần, chạy mọi nơi* (write once, run anywhere).

JVM cung cấp một môi trường thực thi an toàn, nơi nó thực hiện các chức năng tương tự như một hệ điều hành. Nó quản lý bộ nhớ, thực thi các lệnh dựa trên ngăn xếp, và xử lý các kiểu dữ liệu nguyên thủy. Việc này giảm thiểu các rủi ro bảo mật và tăng tính ổn định của ứng dụng.

- *Đơn vị cơ bản của mã Java là lớp (class)*. Trong Java và các ngôn ngữ hướng đối tượng khác, lớp là thành phần ứng dụng chứa mã thực thi và dữ liệu.

- Lớp được lưu trữ và tải một cách động khi ứng dụng cần tới, điều này cho phép Java quản lý hiệu quả các tài nguyên và chỉ tải những gì cần thiết.

- Java mang lại một số tính năng quản lý bộ nhớ tiên tiến để cải thiện an toàn, khả năng di động, và khả năng tối ưu hóa. Java loại bỏ các con trỏ linh tinh có thể tham chiếu tới bất kỳ khu vực nào trong bộ nhớ và thêm thu gom rác (garbage collection) cùng mảng cấp cao vào ngôn ngữ.

- Mặc dù Java không có con trỏ theo nghĩa truyền thống, nó cung cấp các **tham chiếu**, một loại con trỏ an toàn. Tất cả đối tượng trong Java, ngoại trừ các kiểu số nguyên thủy, đều được truy cập qua các tham chiếu. Bạn có thể sử dụng các tham chiếu để xây dựng các cấu trúc dữ liệu thông thường mà một lập trình viên C sẽ làm với con trỏ, nhưng phải theo cách an toàn về kiểu dữ liệu. Khác với con trỏ, bạn không thể sử dụng các thao tác số học trên tham chiếu để thay đổi giá trị của chúng; chúng chỉ có thể chỉ đến các đối tượng cụ thể hoặc các phần tử của mảng. Tham chiếu là một thực thể nguyên tử; bạn không thể thao túng giá trị của một tham chiếu ngoài việc gán nó cho một đối tượng. Sự bảo vệ này là một trong những khía cạnh cơ bản nhất của an ninh Java, đảm bảo rằng mã Java phải tuân theo các quy tắc; nó không thể nhìn trộm vào những nơi không được phép.

## So sánh Java với các ngôn ngữ lập trình khác

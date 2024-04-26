C++程式：新增整合器
獲取user在鍵盤上鍵入的兩個整數，計算他們的總和，並使用std::cout輸出結果。

这段代码是用于 C++ 中的输入输出操作。让我解释一下：

- `std::cout` 是 C++ 标准库中的输出流对象，用于向控制台输出信息。
- `<<` 操作符用于将信息插入到输出流中。
- `"Enter first integer:"` 是一个字符串常量，它将作为提示信息输出到控制台。
- `std::cin` 是 C++ 标准库中的输入流对象，用于从控制台读取用户的输入。
- `>>` 操作符用于从输入流中提取数据。
- `number1` 是一个变量，用于存储从用户输入读取的整数值。

因此，这段代码的作用是向用户显示提示消息 `"Enter first integer:"`，然后从用户输入读取一个整数，并将其存储在变量 `number1` 中。

are declarations,and number1,number2 and sum 是變數的名稱．
變數是計算機記憶體中可以儲存值，供程式使用的位置．
這些宣告指定變數number1,number2 and sum data of type int(integer)such as 7,-11,0 and 31914.
所有變數都必須用名稱和資料型別宣告。

int number1{0};
在變數名稱後面的大括號{}中放一個值，將每個變數初始化為0。
這稱為括號初始化，在c++11中引入
int number{0};
也可以寫成
int number1 = 0;//first integer to add (initialized to 0)
int number2 = 0;//second integer to add (initialized to 0)
int sum = 0;//sum of number1 and number2 (initialized to 0)

在傳統c++程式中，可能會遇到使用這種舊編碼風格的初始化語句。

一次宣告多個變數 Declaring Multiple Variables at Once

同一行別的變數可以在同一個宣告中宣吿

可以使用逗號分隔的列表來宣吿和初始化所有三個變數，如下所示：

int number{0}, number2{0}, sum{0};
然而這使得程式的可讀性降低
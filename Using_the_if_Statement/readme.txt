using Declarations-使用宣告
using std::cout
using std::cin

using不需要重複std::前綴的宣告
在程式的其餘部分簡單地寫cout而不是std::cout和cin而不是std::cin

using Directive-使用指令
using namespace std;
這使程式能夠使用std名稱空間中的名稱，而無需std::資格。

using namespace std; 的作用是將 std 命名空間中的所有成員引入當前的程式碼範圍，
以便你可以直接使用其中定義的函數、類別和物件，而不需要在每次使用時都加上 std:: 前綴。

舉例來說，假設你想使用 std 命名空間中的 cout 和 endl，你可以這樣寫：
#include <iostream>

int main() {
    using namespace std; // 將 std 命名空間引入程式碼範圍
    cout << "Hello, world!" << endl;
    return 0;
}
而不需要寫成：
#include <iostream>

int main() {
    std::cout << "Hello, world!" << std::endl;
    return 0;
}

回到使用std::這被認為是良好做法，可以幫助避免一些微妙的編碼錯誤

Variable Declarations and Reading the Inputs from the User-變數宣告和讀取使用者的輸入

int number1{0};第一個要比較的整數（初始化為0)
int number2{0};第二個要比較的整數（初始化為0)
------------------------------------------------------------------------------------
cin >> number1 >> number2;從使用者那裡讀取兩個整數

uses cascaded stream extraction operations to input two integers.
使用級聯流提取操作來輸入兩個整數。
因為第6行，我們被允許寫cin（而不是std::cin）。
此語句首先將一個值讀入number1，然後將另一個值讀入number2。

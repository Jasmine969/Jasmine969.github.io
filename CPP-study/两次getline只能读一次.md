# 问题描述
```C++
#include <iostream>
#include <string>

using std::cin;
using std::cout;
using std::endl;
using std::string;
using std::getline;

int main()
{
    string s1, s2, judge;
    do
    {
        cout << "Enter the first string:" << endl;
        getline(cin, s1);
        cout << "Enter the second string:" << endl;
        getline(cin, s2);
        cout << "The longer sequence is: " << endl;
        if (s1.size() > s2.size())
        {
            cout << s1 << endl;
        }
        else
        {
            cout << s2 << endl;
        }
        cout << "More? Enter yes or no" << endl;
        cin >> judge;
        // cin.ignore(); // 有一个回车在缓冲区，清除之
    } while (judge[0] == 'y');
    return 0;
}
```

上面的代码，第一轮循环没问题

![](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220307150606.png)

输入`yes`之后，进入第二轮循环，发现根本没有机会键入`s1`的值
![](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220307150853.png)

debug显示：![](https://gitee.com/feng-xiaomo/fengimages/raw/master/20220307150947.png)

# 原因探析

实际上，在`cin >> judge`的时候，输入`yes`，`"yes"`存入`judge`，此时==缓冲区中尚有一个回车符号==。

因此下一轮第一个`getline`的时候，会自动把这个回车读进去，按`getline`的做法，会在存储入`s1`时删去`\n`，因此最后的`s1`就是空字符。

# 解决方案

要避免此种情况发生，只需在`cin >> judge`后添加一句`cin.ignore();`，这样可以把缓冲区的回车清除。
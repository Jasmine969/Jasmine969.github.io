# 不改变实参的交换

## 交换值

```C++
#include <iostream>
using std::cout;
using std::endl;

void swapParamVal(int a, int b)
{
    int tmp = a;
    a = b;
    b = tmp;
    cout << "形参 a b 分别为" << a << ' ' << b << endl;
}

int main()
{
    int x = 1, y = 2;
    cout << "初始 x y 分别为" << x << ' ' << y << endl;
    swapParamVal(x, y);
    cout << "实参 x y 分别为" << x << ' ' << y << endl;
	return 0;
}
```

> 初始 x y 分别为1 2
> 形参 a b 分别为2 1
> 实参 x y 分别为1 2

## 交换指针

```C++
void swapParamPointer(int *pa, int *pb)
{
	int *tmp = pa;
    pa = pb;
    pb = tmp;
    cout << "形参 a b 分别指向" << *pa << ' ' << *pb << endl;
}

int main()
{
    int x = 1, y = 2;
    cout << "初始 x y 分别为" << x << ' ' << y << endl;
    swapParamPointer(&x, &y);
    cout << "实参 x y 分别为" << x << ' ' << y << endl;
	return 0;
}
```

> 初始 x y 分别为1 2
> 形参 a b 分别指向2 1
> 实参 x y 分别为1 2

# 改变实参的交换

## 用引用交换值

```C++
void swapReferVal(int &ra, int &rb)
{
    int tmp = ra;
    ra = rb;
    rb = tmp;
    cout << "形参 ra rb 分别为" << ra << ' ' << rb << endl;
}

int main()
{
    int x = 1, y = 2;
    cout << "初始 x y 分别为" << x << ' ' << y << endl;
    swapReferVal(x, y);
    cout << "实参 x y 分别为" << x << ' ' << y << endl;
    return 0;
}
```

>初始 x y 分别为1 2
形参 ra rb 分别为2 1
实参 x y 分别为2 1

## 交换指针所指的值

```C++
void swapPointedVal(int *pa, int *pb)
{
    int tmp = *pa;
    *pa = *pb;
    *pb = tmp;
    cout << "形参 pa pb 分别指向" << *pa << ' ' << *pb << endl;
}

int main()
{
    int x = 1, y = 2;
    cout << "初始 x y 分别为" << x << ' ' << y << endl;
    swapPointedVal(&x, &y);
    cout << "实参 x y 分别为" << x << ' ' << y << endl;
    return 0;
}
```

> 初始 x y 分别为1 2
> 形参 pa pb 分别指向2 1
> 实参 x y 分别为2 1

## 用引用交换指针

```C++
void swapReferPointer(int *&rpa, int *&rpb)
{
	int *tmp = rpa;
    rpa = rpb;
    rpb = tmp;
    cout << "形参 rpa rpb 分别指向" << *rpa << ' ' << *rpb << endl;
}

int main()
{
    int x = 1, y = 2;
    int *p = &x, *q = &y;
    cout << "初始 x y 分别为" << x << ' ' << y << endl;
    swapReferPointer(p, q); // 不能给字面值绑定引用，所以这边必须传入变量p和q
    cout << "实参 p q 分别指向" << *p << ' ' << *q << endl;
    cout << "实参 x y 分别为" << x << ' ' << y << endl;
    return 0;
}
```

> 初始 x y 分别为1 2
> 形参 rpa rpb 分别指向2 1
> 实参 p q 分别指向2 1
> 实参 x y 分别为1 2

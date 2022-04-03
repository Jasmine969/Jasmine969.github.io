首先定义一个字符变量`c`

想用`cin`读入一段文本，包括换行符

- 用`cin >> c`肯定不行，这个连空格都统计不了，更别说换行符了

- 用`getline(cin, c)`也不行，换行符虽然能读取，但是保存的时候会被丢弃

- 用`cin.get(c)`才是正确做法！！用这个能读入制表符、换行符、空格

  ```C++
  char c;
  int newlineCnt = 0;
  while (cin.get(c))
  {
      if (c == '\n')
          ++newlineCnt；
  }
  ```

  
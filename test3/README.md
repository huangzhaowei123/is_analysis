# 实验三：图书管理系统领域对象建模

|学号|班级|姓名|
|:----:|:----:|:----:|
|201510414112|15级软工一班|黄照伟|

# 1.图书管理系统类图
### 1.1类图源码：
```
@startuml

class 读者{
    -ID:String
    -name:String  
    -sex:String
    -role:String 
    -number:Interger
}
class 注册用户{
    -ID:String
    -name:String  
    -sex:String
    -role:String 
    -number:Interger
}
class 会员{
    -name:String 
    -age:Interger
    -maxBorrowNum:Interger
    -maxBorrowDays:date
    -roletime:date
}
class 预定的记录{
    -booktime:date
    +add()
    +select()
}
class 借书记录{
    -lendtime:date
    -returntime:date
    +add()
    +select()
}
class 逾期记录{
    -continueday:date
    -lastday:date
    -returntime:date
    +add()
    +select()
}
class 超级管理员{
    -mangerId:Interger
    -mangerName:String
    -mangerNumber:String
    -mangerAddress:String
    -mangerPhone:String
    +add()
    +select()
    +delete()
    +update()
}
class 管理员信息{
    -mangerId:Interger
    -mangerName:String
    -mangerNumber:String
    -mangerAddress:String
    -mangerPhone:String
    +add()
    +select()
    +delete()
    +update()
}
class 读者信息{
    -readerId:Interger 
    -readerName:String 
    -bookISBN:String 
    -lendBookTime:String 
    -returnBookTime:String
    +select()
    +borrow()
    +xujie()
    +yujie()
    +returnBook()
    +findBook()
}
class 图书信息{
    -bookId:Interger
    - bookISBN:String
    -bookName:String 
    -total:Interger 
    -stock:Interger 
    -publisher:String 
    -author:String 
    -summary:String
    +add()
    +select()
    +delete()
    +update()
    +setStatus()
}

读者信息 "多" --* "1" 预定的记录  :借阅
读者信息 --> 借书记录:添加
借书记录 --> 管理员信息:增加借阅信息
借书记录 --> 逾期记录
逾期记录 --> 管理员信息:处理
预定的记录 --> 管理员信息 :增加预定记录
管理员信息 "1" --* "多" 图书信息 :mange
管理员信息 "1" --* "多" 读者信息  :mange
超级管理员 "1" -- "多"管理员信息:contains
读者信息    <|--    读者
读者信息    <|--    注册用户
读者信息    <|--    会员

@enduml

```
### 1.2类图

![](./1.png '描述')

# 接口：getCourse  [返回](../README.md)
用例： [选课](../yongli/选课.md)

- 功能：
    学生选择一门课程。
    
- 权限：
    必须已学生的身份登录
    
- API请求地址： 
    接口基本地址/v1/api/getCourse/<teacher_id>

- 请求方式 ：
    GET

- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |student_id|学生的学号|
    
- 返回实例：

        {         
           "name":"数值计算";
           "introduce":"这是一门***********";
        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |name|课程名称|
  |introduce|课程介绍|
 



<a name="paths"></a>
## 资源

<a name="book-controller_resource"></a>
### Book-controller
Book Controller


<a name="postbookusingpost"></a>
#### 创建图书
```
POST /books
```


##### 说明
创建图书


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Body**|**book**  <br>*必填*|图书详细实体|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|string|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/books
```


###### 请求 body
```
json :
{ }
```


##### HTTP响应示例

###### 响应 200
```
json :
"string"
```


<a name="getbookusingget_1"></a>
#### 获取图书列表
```
GET /books
```


##### 说明
获取图书列表


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|< [Book](#book) > array|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/books
```


##### HTTP响应示例

###### 响应 200
```
json :
[ {
  "id" : 0,
  "name" : "string",
  "price" : 0.0
} ]
```


<a name="getbookusingget"></a>
#### 获图书细信息
```
GET /books/{id}
```


##### 说明
根据url的id来获取详细信息


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Path**|**id**  <br>*必填*|ID|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|[Book](#book)|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/books/string
```


##### HTTP响应示例

###### 响应 200
```
json :
{
  "id" : 0,
  "name" : "string",
  "price" : 0.0
}
```


<a name="putuserusingput"></a>
#### 更新信息
```
PUT /books/{id}
```


##### 说明
根据url的id来指定更新图书信息


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Path**|**id**  <br>*必填*|图书ID|string|
|**Body**|**book**  <br>*必填*|图书实体book|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|string|
|**201**|Created|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|
|**404**|Not Found|无内容|


##### 消耗

* `application/json`


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/books/string
```


###### 请求 body
```
json :
{ }
```


##### HTTP响应示例

###### 响应 200
```
json :
"string"
```


<a name="deleteuserusingdelete"></a>
#### 删除图书
```
DELETE /books/{id}
```


##### 说明
根据url的id来指定删除图书


##### 参数

|类型|名称|说明|类型|
|---|---|---|---|
|**Path**|**id**  <br>*必填*|图书ID|string|


##### 响应

|HTTP代码|说明|类型|
|---|---|---|
|**200**|OK|string|
|**204**|No Content|无内容|
|**401**|Unauthorized|无内容|
|**403**|Forbidden|无内容|


##### 消耗

* `application/json`


##### 生成

* `*/*`


##### HTTP请求示例

###### 请求 path
```
/books/string
```


##### HTTP响应示例

###### 响应 200
```
json :
"string"
```




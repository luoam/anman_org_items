# anman_org_items
将失踪儿童的信息存上星云链

### 功能介绍
 1. 预设超级管理员
 2. 注册志愿者
 3. 失踪儿童信息维护
 4. 日志记录


# 全部可用方法介绍：
#### 志愿者：
#####  1. 添加志愿者
<pre>
AddAdmin: function (address, beizhu) {}
</pre>
##### 2. 删除志愿者
<pre>
DelAdmin: function (address) {}
</pre>
##### 3. 查看全部志愿者
<pre>
GetAdmins: function () {}
</pre>

#### 失踪儿童信息维护：
##### 1. 添加失踪儿童信息
<pre>
AddChildItem: function (itemid, name, agesex, misslocation, misstime, photos, detail, policeman, policetel, status, close, misscheme, suspect) {}
</pre>
##### 2. 删除失踪状态已找回的信息
<pre>
DelChildItem: function (itemid) {}
</pre>
##### 3. 返回全部失踪儿童的信息
<pre>
GetChildItems: function (limit,offset) {}
</pre>
##### 4. 返回具体某个失踪儿童的信息
<pre>
GetChildItem: function (itemid) {}
</pre>
##### 5. 返回全部失踪儿童的itemid
<pre>
GetItems: function () {}
</pre>

#### 日志信息
默认对每一次调用都会记录一次日志
##### 1. 获取日志
<pre>
GetLogs: function () {}
</pre>
##### 2. 返回总的调用次数
<pre>
GetCount:function () {}
</pre>

#测试：
 1. 添加志愿者&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;通过
 2. 查看志愿者列表&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;通过
 3. 删除志愿者&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;通过
 4. 添加失踪儿童信息&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;通过
 5. 返回全部失踪儿童的信息&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;通过
 6. 删除失踪儿童信息&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;通过
 7. 返回具体某个失踪儿童的信息&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;通过
 8. 返回全部失踪儿童的itemid&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;通过
 9. 获取日志&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;通过
 10. 返回总的调用次数&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;通过
 11. 注册成为志愿者&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;通过
 
#页面包括三个
 1. 首页 
 2. 登记成为注册志愿者
 3. 失踪儿童数据上链
 
####首页： 
 从星云链上获取失踪儿童的数据，并加载到页面上。 
 在使用时，请将页面中的initAddress换成自己的星云钱包地址：
 <pre>
 var initAddress = "自己的星云钱包地址";
 </pre>
 
####登记成为注册志愿者：

 效果如：http://www.anman.org/nebulas/regvolunteer
 
####失踪儿童数据上链
  这个需要先注册成志愿者之后才可以操作，主要看公安部失踪儿童紧急信息发布平台与星云链上的失踪儿童数据差异，根据差异进行上链操作。
 
# Tmall
天猫商城项目JavaEE实现  

<b>java源代码包结构:  </b>  
tmall.bean 实体类  
tmall.comparator 比较器  
tmall.dao DAO类  
tmall.filter 过滤器  
tmall.servlet servlet  
tmall.test 测试类  
tmall.util 工具类  

<b>web目录:</b>  
css css文件  
img 图片资源  
js js文件  
admin 后台管理用到的jsp文件  
include 被包含的jsp文件  

<b>经过这个项目，我们都完成了如下的一系列典型场景功能:</b>  
1. 购物车: 立即购买 加入购物车 查看购物车页面 购物车页面操作  
2. 订单状态流转: 生成订单 确认支付 后台发货 确认收货 评价  
3. CRUD增删改查: 后台各种功能  
4. 分页: 后台各种功能  
5. 一类产品多属性配置: 属性管理  
6. 一款产品多图片维护: 产品图片管理  
7. 产品展示:  前台首页 前台产品页  
8. 搜索查询  
9. 登录、注册、退出  
10. 登录验证  
# 设计模式：
1. MVC  
MVC设计模式贯穿于整个后台与前台功能开发始末  

2. Filter+Servlet+反射  
采用Filter+Servlet+反射的设计模式，  
把原本后台需要20多个Servlet的经典Servlet设计方式，精简到了7个。  
把原本前台需要20多个Servlet的经典Servlet设计方式，精简到了2个。  
web.xml的配置文件也大大减少，降低了开发和维护的工作量，减少了出错的几率。  

3. 统一的分页查询简化开发  
所有的后台都使用同一个分页机制，仅仅需要一份简化的adminPage.jsp即满足了各种分页功能的需求，简化了开发，提升了开发速度。  

4. 模块化JSP设计  
从大的JSP文件中，通过JSP包含关系抽象出多个公共文件，并把业务JSP按照功能，设计为多个小的JSP文件，便于维护和理解  

### 功能概述
* 从 超玩业务-首页 的入口进入
* 用户的个人中心，实际上只有 我的订单，超玩看到才是完整版
* 返回点击后，回到超玩列表首页
* 了解完整的 [订单状态](order-state.md)

### 原型
![](img/个人中心-用户.jpg)

### 1. 订单状态
* 不同订单状态，对应不同功能
* 同样的状态，超玩可能没有操作的功能，这是两者的区别
* 功能内藏在 `更多`（水平3点的icon） 里

#### 1.2 状态对应的功能
* 等待响应
	* 功能：取消订单
	* 进行二次确认
* 沟通阶段
	* 功能：取消订单
	* 进行二次确认
* 进行中
	* 功能：结束订单
	* 进行二次确认
* 已完成
	* 功能：我要申诉
		* 显示联系客服的方式
	* 功能：评价订单
		* 进入 进行评价 页面
		* 评价完成后，取消按钮显示
* 已取消
	* 无功能

### 2. 订单时间的显示
订单时间和订单状态有对应关系

* 等待响应  ——  显示 支付成功 时间
* 进行中  ——  显示 订单开始 时间
* 已完成  ——  显示 订单完成 时间
* 已取消  —— 显示 订单取消 时间

### 3. 更多 按钮的展开样式
点击 `更多`（水平3点的icon）后，会原地展开

![](img/菜单-更多.jpg)

点击非按钮区域，收起

### 4. 取消订单的确认菜单
![](img/菜单-取消订单-确认.jpg)

必须选择一个理由

没有选择时，会toast提示用户，必须选择一个理由

![](img/提示-toast.jpg)

### 5. 结束订单的确认菜单
![](img/菜单-结束订单-确认-用户.jpg)

点击后订单状态变为 `已完成`


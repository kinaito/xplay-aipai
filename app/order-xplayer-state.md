### 功能概述
* 超玩的接单状态
* 超玩可手动改变自己的接单状态
* 当前有4种状态：休息、服务中、忙碌、冻结


### 1. 休息
相当于离线状态

* 可手动切换到该状态
* 用户不可对该状态的超玩下单
* 不会收到新订单
* 不会在任何地方推荐显示

		超玩可手动切换

### 2. 服务中
相当于可接单状态

* 用户可对该状态的超玩下单
* 收到新订单
* 会在任何地方推荐显示
* 收到新订单时，直到超玩响应，系统自动将其接单状态切换到 **`忙碌`**
* 如果连续2次60秒内不响应订单，会因超时响应，系统警告并将超玩的接单状态切换到 **`休息`**

		超玩可手动切换

### 3. 忙碌
* 超玩不可手动切换到该状态
* 用户不可对该状态的超玩下单
* 不会收到新订单
* 不会在任何地方推荐显示
* 收到新订单时，会进入该状态
* 开始订单时，会进入该状态
* 订单结束后，系统将状态切换到 **`服务中`**

		进入此状态时，超玩不能手动切换状态

### 4. 冻结
* 超玩不可手动切换到该状态
* 用户不可对该状态的超玩下单
* 不会收到新订单
* 不会在任何地方推荐显示

		进入此状态时，超玩不能手动切换状态
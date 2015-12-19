# www.sxg.com
## 收藏

### 我的收藏

```
/**
 * 收藏
 * http://www.sxg.com/user/mycollect/token/2a26d06f38e4f13cdcf5e8da18777993/tid/1
 * @return [type] [description]
 */
```

### 添加收藏

```
/**
 * 收藏
 * @param int zid 综合id
 * @param int tid 类型id 2为百科,1为商品
 * @param string token
 * http://192.168.0.188/www.sxg.com/comm/collect/token/2a26d06f38e4f13cdcf5e8da18777993/zid/9/tid/2
 * @return [type] [description]
 */
```

## 点赞

```
/**
 * 点赞
 * @param int zid 综合id
 * @param int tid 类型id 0为百科,1为吐槽,2为问答
 * @param string token
 * @param int type 点赞类型,0为good 1为bad
 * http://192.168.0.188/www.sxg.com/comm/sup/token/2a26d06f38e4f13cdcf5e8da18777993/zid/9/tid/2/type/1
 * @return [type] [description]
 */
```

## 评论

### 首页

```
/**
 * show
 * @param int zid 综合id
 * @param int tid 类型id 0为百科,1为吐槽,2为问答
 * http://www.sxg.com/discuss/index/token/2a26d06f38e4f13cdcf5e8da18777993/zid/5/tid/1
 * @return [type] [description]
 */
```

### 添加评论

```
/**
 * 添加评价add
 * @param int zid 综合id
 * @param int tid 类型id 0为百科,1为吐槽,2为问答
 * @param string token
 * @param string content 评论内容
 * 2a26d06f38e4f13cdcf5e8da18777993
 */
```
## 百科

### 百科首页

```
http://192.168.0.188/www.sxg.com/article/index/token/2a26d06f38e4f13cdcf5e8da18777993/p/0/t/1
token
p:分页
t:分类id
```
### 百科详情

```
http://192.168.0.110/www.sxg.com/article/getinfo/token/2a26d06f38e4f13cdcf5e8da18777993/id/11
eoken
id:百科id
```

## 问答吐槽

### 问答吐槽首页

```
/**
 * show
 * @param int t 类型 2:吐槽 3:问答
 * @param int p 页码
 * http://www.sxg.com/Teasing/index/t/2/p/1
 * @return [type] [description]
 */
```

### 添加问答吐槽

```
/**
 * +----------------------------------------------------------
 *  添加问答/吐槽
 *  http://192.168.0.110/www.sxg.com/index.php/Teasing/add/token/2a26d06f38e4f13cdcf5e8da18777993/type/1
 * @param  Int type    类型 1:吐槽 2:问答 get
 * @param  String  token   
 * @param  String  title   标题
 * @param  String  content 内容
 * +----------------------------------------------------------
 */
```

## 收货地址

### 添加收货地址

```
/**
 * 添加收货地址
 * http://192.168.0.110/www.sxg.com/user/addAddress/token/2a26d06f38e4f13cdcf5e8da18777993/
 * @param phone   手机号码
 * @param string area   区
 * @param string city  市
 * @param string province 省
 * @param string consignee  收货人
 * @param int isdefault    是否默认
 */
```

### 删除收货地址

```
/**
 * http://192.168.0.110/www.sxg.com/user/delAddress/token/2a26d06f38e4f13cdcf5e8da18777993/
 * @param int id  搜获地址id
 * @return [type] [description]
 */
```

### 修改收货地址

```
/**
 * http://192.168.0.110/www.sxg.com/user/saveAddress/token/2a26d06f38e4f13cdcf5e8da18777993/
 * @param int id  收货地址id
 * @param phone   手机号码
 * @param string area   区
 * @param string city  市
 * @param string province 省
 * @param string consignee  收货人
 * @param int isdefault    是否默认
 * @return [type] [description]
 */
```

### 显示收货地址

```
/**
 * 显示收货地址
 * http://192.168.0.110/www.sxg.com/user/saveAddress/token/2a26d06f38e4f13cdcf5e8da18777993/
 * @param token
 * @return [type] [description]
 */
```

## 订单管理

### 添加订单

```
/**
http://192.168.0.110/www.sxg.com/order/add/token/2a26d06f38e4f13cdcf5e8da18777993
 * 添加订单 add
 * token
 * consignee 收货人
 * country 国家
 * province 省份
 * city 市
 * district 地区
 * address 详细地址
 * mobile 手机
 * email 邮箱
 * best_time 最佳送货时间
 * postscript 留言
 * pay_id 支付ID
 * array goods = array(
 *                 [0] => array(
 *                     'goods_id' => 1,
 *                     'goods_number' => 1,
 *                 ),
 *                 [1] => array(
 *                     'goods_id' => 2,
 *                     'goods_number' => 3,
 *                 ),
 *                 ......
 *             )
 *
 */
``` 

### 查看订单/订单详情

```
/**
 * 获取用户订单
 * http://192.168.0.110/www.sxg.com/order/get/token/2a26d06f38e4f13cdcf5e8da18777993
 * @return [type] [description]
 */
```
### 删除订单

```
/**
* 删除
* @param order_id get
* @return [type] [description]
* http://192.168.0.110/www.sxg.com/order/del/token/2a26d06f38e4f13cdcf5e8da18777993
*/
```

## 商品

### 商品排序

```
http://192.168.0.110/www.sxg.com/goods/index/type/desc/desc/goods_number/cat_id/1/page/0

type:`desc 降序`
	 `asc  升序`
desc:`goods_id     商品添加时间`
	 `market_price 市场售价`
	 `shop_price   本店售价`
cat_id:分类id
page:分页
```

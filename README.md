# 凡信-最强微信仿品 #
## 2016年2月更新 ##
###凡信的第一个版本于2015年4月份发布，之后由于自己工作忙碌的原因，一直没有重大的更新内容。2016年1月份抽空做了一些更新。主要是加入了朋友圈和钱包这两块内容，以及对第一版的一些bug的修复。凡信2.0依然是基于环信IM通信云SDK开发的，当前状态下第三方通信云趋于火热，环信也这一年走过四轮共计几千万美元的融资，开发者用户也呈现几万的增长。这个项目也算是给需要集成IM云的开发者提供一个参考，给刚接触Android开发，对Android整体开发框架还很模糊同学提供一个学习的教材。 ###
### 关于此次更新的朋友圈版块，有些地方的处理的我觉得非常有技术分享的价值，项目为了极速开发，整个项目写得有点凌乱粗糙，但是部分功能单独拎出来讨论。会以博客的形式的解析一些功能。 ###
##   
    作者QQ : 84543217
    技术讨论群：437758366（已有900名小伙伴等着你） ##
#### **一、朋友圈相关** ####


1. 发布动态--文字 图片 位置
2. 朋友动态列表
3. 点赞
4. 评论
5. 识别网址
6. 好友的所有动态查看
7. 我的相册
8. 部分功能待完善
#### **二、钱包相关** ####
1. 零钱 -虚拟账户
2. 充值 选择卡-充值-每张卡初始额度200元
3. 提现 提现到卡-需要手动处理才能完成，我就不手动去弄了，因此提现后无法到你的卡（注：此卡指的是凡信中的虚拟卡）
4. 交易记录---转账、充值、提现三类
5. 银行卡 后台虚拟了一些卡账号，每张卡有200的额度。添加后可充值
6. 给好友转账--后面会添加提现和在聊天页显示。     
7. 支付宝集成(app中常用的功能)-----集成了支付宝的SDK，由于密钥等参数都是比较重要的，已在工程中去掉了。体验这个带参数的功能，可以下载这个包-http://120.24.211.126/fanxin/download/Fanxin.apk，做了一个打赏的功能。
#### **三、  逻辑变化：** ####
好友关系独立化，弃用了环信的好友关系表，在后端自己管理好友关系，这样做是跟朋友圈的业务相关，因此请务必注册新的账号的测试。
### 2015年 4月更新 ###
1.注册登录部分：<br>
     1.1重写了EditText的默认的蓝色底线，变成微信的绿色<br>
     1.2 登录和注册按钮对输入框进行监听，并变色<br>
     1.3 密码明文和隐藏<br>

2.主页<br>
     2.1全仿微信底部导航<br>
     2.2 右上角加号按钮可进入 “发起群聊”和“添加朋友“<br>
     2.3 显示未读消息数和未读通知数<br>
3.聊天列表页：<br>
     3.1 群聊头像是群成员头像的组合，有1.2.3.4.5种类型的头像<br>
     3.2 置顶功能。置顶后该会话item置于列表顶端，并像微信一样变底色<br>
     3.3 删除列表功能，删除该条会话记录<br>
4.通讯录页<br>
     4.1 显示好友列表<br>
     4.2 进入还有申请通知<br>
     4.3 进入群聊列表<br>
5.发现页（正在开发朋友圈功能.....）<br>
6.用户详情页<br>
      6.1 资料设置（目前可更改的资料是：头像、昵称、性别）<br>
      6.2 微信号只能设置一次。<br>
      6.3 设置页（通知、声音、震动、退出登录）<br>
7.用户申请通知<br>
      7.1按时间由近及远排序<br>
      7.2 显示申请理由<br>
      7.3 处理状态（已添加、同意）<br>
8.查找添加用户<br>
      8.1 按用户的手机号查找用户<br>
      8.2 搜索的用户的存在显示用户资料<br>
      8.3 若该用户已经是好友，显示”发送消息“按钮<br>
      8.4 若该用户不是好友，显示添加好友，并要求输入申请理由<br>
9.发起群聊<br>
      9.1可以在输入框内按用户昵称搜索好友<br>
      9.2 添加群聊的用户的头像可以动态显示在顶部<br>
10.聊天页面<br>
      可以发送语音文字图片和视频（后续更新更多表情和设置聊天背景）<br>
11聊天设置<br>
       11.1单聊：置顶聊天、免打扰、和清除聊天记录<br>
       11.2 群聊：显示群成员列表、增加群成员、删除群成员（群主可操作）、
                  修改群名称、置顶聊天、屏蔽清除群消息<br>
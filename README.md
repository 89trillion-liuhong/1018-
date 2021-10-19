每日精选
  整体框架
    通过simplejson读取数据，并显示在UI上，主要通过判断json的数据源补充对应的UI。UI实现对应点击效果


  界面拆分结构
    Hierarchy：
      MainCamera
      canvans{
        image(背景)
        scrollview
          shopitem
      }

  代码结构
    UImananger(根据jsonmanager读取对象列表)
    jsonmannger（读取json创建相应对象）
    shopItem(对象属性)
    OnButtonDown(点击事件)

  预制物
    coinPrefab（金币部分），shopItemPrefab（卡牌部分）,emptyPrefab（空白上锁部分）

士兵招募
  整体框架
    通过button实现点击生成金币，在使用DoTween移动金币

  界面结构
    maincamera
    canvans
      openbox
      closebox
      button

   代码结构
    OnButtonDown(当玩家点击，显示/隐藏 图片。根据点击次数生成金币)
    coin（使用DoTween移动位置，通过协程改变图片）
   预制物
    coinPrefab

2.动画
  整体框架
    使用状态极修改播放动画，读取csv文件实现相应机制
  界面结构
    maincamera
    canvan
      player
        hp_bar
      enemy
        hp_bar
        
   代码结构
    OnButtonDown(事件触发)
    person(人物基类)
    player(玩家类)
    enemy(敌人类)
    
    
    
      
   
    
    

# Battleship
mini game
根据head first javascript写了一个小游戏，将之前学到的东西融合汇总
## 游戏描述
随机生成三个长度为三格的战舰，用户输入猜测的位置坐标，浏览器显示是否正确，在网页上显示战舰或者miss，并记录猜测次数，在上方的文本栏显示文字提示。
## HTML与CSS
背景黑色，并设置背景图中格子的大小与html中格子大小相同，难度较小。
分别建立击中和未击中两个类的样式，在后面的js中可以通过修改元素的类来显示图像。
## 对象设计
#### 显示界面view
用于更新页面，主要可以分为三个方法，消息栏的内容显示以及击中未击中的显示。
使用DOM获取id相对应的元素，并修改值。setAttribute（"标签"，"标签值"），设置标签，即可显示。
#### 模型对象 model
存储游戏状态，修改状态
设置属性：网格数量 战舰数量 战舰位置 已击沉战舰数 战舰长度 
方法：判断是否被击中
#### 控制对象
获取玩家的输入，并记录次数
## 设置战舰放置方式
创建战舰，确定战舰方向（水平 垂直），根据第一个位置生成后两个位置，判断战舰之间不重合，保存至数组

## 总结
这个小游戏让我认识到了面向对象编程的思路，之前一直都是面向过程编程，面向对象还是不太习惯。从这个游戏来说应该从整体考虑，大致包括显示部分，输入部分，以及
游戏的部分。在编码过程中遇到了一些问题，主要是经常把：写成=，区别应该是：表示子，=表示赋值，还需要多加练习。写这个小游戏熟悉了一些常用方法，包括push（），
charAt（），indexOf（），Attribute(),isNaN()...

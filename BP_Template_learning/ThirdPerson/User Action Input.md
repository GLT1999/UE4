#### FirstPerson/ThirdPerson

```c++
/*
User Action Input
键盘绑定：LookUp:Scale:-1 Turn:Scale:1
	 	MoveForward:W:1 S:-1 MoveRight:A:-1 D:-1
事件学习：InputAxis Ture/InputAxis LookUp
		InputAxis MoveForward/InputAxis MoveRight
		InputAction Jump
		Event Bluprint Update Animation
函数学习：Add Controller Yaw Input
		Add Controller Pitch Input
		Add Movement Input
		Jump/Stop Jump
纯函数学习：Get Controller/Get Control Rotation/Break Rotator/Make Rotator
		  Get Forward Vector(Pawn) / Get Actor Forward Vector
		  Try GetPawn Owner
		  (GetMovement Component / is Falling
		  (Get Velocity / VectorLength		
*/
```

![image-20210525155226796](C:\Users\GLT1999\AppData\Roaming\Typora\typora-user-images\image-20210525155226796.png)

#### Animation：设置speed

**![image-20210524214343967](C:\Users\GLT1999\AppData\Roaming\Typora\typora-user-images\image-20210524214343967.png)**

```c++
/*
Get Actor Forward Vector与 Get Forward Vector的区别？
解析：
同样是用于player,InputAxis MoveForward事件，
不同的是Get Actor Forward Vector主要用于mesh与camera绑定，例如第一人的情况，
而Get Forward Vector主要用于mesh与camera分离的情况，例如第三人称的情况；
*/
```

```c++
/*
--补充：节点类型颜色
红色->事件的定义
蓝色->调用的函数或事件
绿色->纯函数
紫色->构造函数定义
青色->对象转换
灰色->宏
*/
```


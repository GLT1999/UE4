#### User Action Input

```c++
/*
设置：LookUp:Scale:-1 Turn:Scale:1
	 MoveForward:W:1 S:-1 MoveRight:A:-1 D:-1
*/
Axis Input
    InputAxis Ture  ->Add Controller Yaw Input
    InputAxis LookUp->Add Controller Pitch Input
    InputAxis MoveForward->Add Movement Input
    (Get Control Rotation->Break Rotator:Z->Make Rotator:Z->GetForward Vector)
    InputAxis MoveRight->Add Movement Input
    (Get Control Rotation->Break Rotator:Z->Make Rotator:Z->GetRight Vector)
Actoin Input
    InputAction Jump->Jump/Stop Jumping
```

#### Animation：设置speed

**![image-20210524214343967](C:\Users\GLT1999\AppData\Roaming\Typora\typora-user-images\image-20210524214343967.png)**

```c++
Event Bluprint Update Animation
    is Valid->Try Get Pawn Owner->GetMovementComponent->is Falling->set(is inAir)
    					    ->Get Velocity->vectorLength->set(speed)
```


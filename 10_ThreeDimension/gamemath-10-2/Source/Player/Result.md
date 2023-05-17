## 예제 실행 결과
![image](https://github.com/pumfit/GameMath/assets/46295539/823012a2-2da7-45fa-a3c0-21ec3dc7d1ee)

### ✈️ yaw, roll, pitch
![image](https://github.com/pumfit/GameMath/assets/46295539/6860a5d9-ff6d-4d09-998c-f51796c0c860)
🔗 https://howthingsfly.si.edu/media/roll-pitch-yaw

|Term|Description|
|---|---|
|yaw | 비행기의 선회 여부를 나타내는데 사용됩니다.|
|roll | 비행기가 수평으로 돌아가는 정도를 나타냅니다.| 
|pitch | 비행기의 고정익이 위아래로 동작하는 정도를 나타냅니다.| 

### 🔓 짐벌 락 현상(Gimbal lock)

오일러 각을 사용하여 3차원 공간의 회전을 다루는 경우 회전 움직임이 제한되는 현상
X,Y,Z 축 중 두 축이 병렬이 되는 경우 다른 한 축이 변경되어도 한 축이 잠긴 상태가 되어 회전 움직임이 제한되는 현상이다.

[![image](https://github.com/pumfit/GameMath/assets/46295539/bf39c900-00ff-48df-baaf-78d63f12f6ec)](https://en.wikipedia.org/wiki/File:Gimbal_Lock_Plane.gif)

이와 같은 짐벌락 현상을 방지하기 위해서는 로드리게스 회전 공식 또는 사원수를 사용한 쿼터니언을 사용하여 방지해야한다.

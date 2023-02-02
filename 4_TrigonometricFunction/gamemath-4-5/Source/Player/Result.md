## 예제 실행 결과
![4_5_1](https://user-images.githubusercontent.com/46295539/215776461-d6db3fdc-5650-4fcb-82a1-021b3b96b0a7.png)


![4_5_2](https://user-images.githubusercontent.com/46295539/215776409-81e99455-0936-4d13-952a-aa3ac63df8e2.png)


![4_5_3](https://user-images.githubusercontent.com/46295539/215776489-b2121435-a68e-4947-af89-b6fa01097cd1.png)

각이 커질 수록 원에 가까워지는 모습을 볼 수 있다.

### 극좌표계

벡터의 크기와 각도로 극좌표계를 `Vector2(Size(),Angle())` 표현할 수 있다.

- size()^2 = x^2 + y^y

- angle = atan2(y,x);

### atan atan2

인자 하나로 atan(y/x)을 쓰거나 atan2(y,x)를 쓸 수 있다.


atan, atan2 함수는 평면의 모든 사분면에 대응하는 각도를 얻을 수 있으며 공역은 (-180,180) 을 가진다.

🔗 https://learn.microsoft.com/ko-kr/dotnet/api/system.math.atan2?view=net-7.0

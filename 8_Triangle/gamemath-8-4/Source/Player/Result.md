## 예제 실행 결과

![8_4_1](https://user-images.githubusercontent.com/46295539/236481897-1337186b-8ce0-42a1-be78-bca7c194a8d4.png)

![8_4_2](https://user-images.githubusercontent.com/46295539/236484721-5b952b56-e29b-4bcf-85e7-1c1bdce36a4c.png)

### 텍스처 매핑
 - texture - 메시에 이미지를 입히기 위해 변환된 데이터
 - texture - mapping 메시에 이미지를 입히는 작업
### 📌 GetSample()
텍스처에서 UV 좌표를 통해 색상을 픽셀에 반영하는 함수

```

LinearColor Texture::GetSample(Vector2 InUV) const
{
	if (!IsIntialized())
	{
		return LinearColor::Error;
	}

	int x = Math::FloorToInt(InUV.X * _Width) % _Width;
	int y = Math::FloorToInt(InUV.Y * _Height) % _Height;
	int index = _Width * (_Height - (1 + y)) + x; // UV 좌표값을 통해 텍스처 버퍼내 인덱스를 얻어온다.
	if (index >= _Buffer.size()) 
	{
		return LinearColor::Error;
	}

	return _Buffer[index];
}
```

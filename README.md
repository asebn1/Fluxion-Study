# Fluxion-Study
Fluxion : Wi-Fi password stealing



```bash
git clone https://github.com/FluxionNetwork/fluxion.git
```

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/2d5c77ae-06b5-4904-98d4-4af119c23730/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/2d5c77ae-06b5-4904-98d4-4af119c23730/Untitled.png)

```bash
cd fluxion
sudo ./fluxion.sh -i
```

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/2713b52b-13f5-4fe5-8812-1d7a7fb97418/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/2713b52b-13f5-4fe5-8812-1d7a7fb97418/Untitled.png)

언어 설정 후 2번(WPA/WPA2 선택)

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/e0400d2f-cc5f-49f9-ab1c-49b73ff1259c/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/e0400d2f-cc5f-49f9-ab1c-49b73ff1259c/Untitled.png)

→ 모니터 모드 WLAN 확인

- 오류는 아닌데 패킷이 안잡히는중.

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/0ae16e38-2357-423a-b749-7d90bec28343/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/0ae16e38-2357-423a-b749-7d90bec28343/Untitled.png)

- 먼저 모니터모드 자동변경 확인

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/e7f1c77e-32cb-42a1-ac16-7b8d39da0768/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/e7f1c77e-32cb-42a1-ac16-7b8d39da0768/Untitled.png)

```bash
airmon-ng start fluxwl0
airmon-ng check kill
```

- 위 명령어 실행 후 하니 잘 잡힘

- control + c 하면 아래와같이 뜸

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6b7b852e-29a0-4e13-969c-99a935df1733/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6b7b852e-29a0-4e13-969c-99a935df1733/Untitled.png)

- 번호 선택 후 2번(skip 선택)

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/aa7bd4ce-ca17-42e1-83b2-66d49ebc9f43/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/aa7bd4ce-ca17-42e1-83b2-66d49ebc9f43/Untitled.png)

- 2번 aireplay-ng deauthentication

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c4fe3d8e-8910-416c-a651-0b6d742d15f8/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c4fe3d8e-8910-416c-a651-0b6d742d15f8/Untitled.png)

- 1번

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d49532e9-bf00-49f4-8fb7-379e335d5126/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d49532e9-bf00-49f4-8fb7-379e335d5126/Untitled.png)

- 얼마나 자주볼건지? → 1번

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/775f4cff-0459-4118-904c-c55be83b5e5c/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/775f4cff-0459-4118-904c-c55be83b5e5c/Untitled.png)

- 2번

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/777ec0bb-3fad-4d82-bf8a-515743de0bb8/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/777ec0bb-3fad-4d82-bf8a-515743de0bb8/Untitled.png)

- 여러번 다른 것 시도해보다가 여기서 막힘

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5d49509d-2bce-46fc-9126-132ba4fb05bc/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5d49509d-2bce-46fc-9126-132ba4fb05bc/Untitled.png)

- virtualBox 에서 패킷 잡다보면 잡힐때도 있고 안잡힐때도 있어서 너무 시간 오래걸림. 한번 시도할때마다 재시도할때 많음.. 그래서 그냥 가상머신 말고 자체 칼리로 시도함

### 선택한 wifi 해쉬값 얻기 성공

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/977808ff-79c6-44df-8448-d390deca31c1/Screenshot_2020-09-17_01-19-55.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/977808ff-79c6-44df-8448-d390deca31c1/Screenshot_2020-09-17_01-19-55.png)

### SSL 인증파일 생성

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/037d5b26-5a45-44d4-b1fd-041b5c6ccf51/Screenshot_2020-09-17_01-24-38.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/037d5b26-5a45-44d4-b1fd-041b5c6ccf51/Screenshot_2020-09-17_01-24-38.png)

### 영어로

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/12ec7335-0636-41c4-b5ba-98f3572cebbd/Screenshot_2020-09-17_01-25-25.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/12ec7335-0636-41c4-b5ba-98f3572cebbd/Screenshot_2020-09-17_01-25-25.png)

### ㅋㅋDEAUTH만 되고 또 계속안됨 ㅎㅎ

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/fa274b12-8ee7-41f7-94df-5d9aafc28ff2/Screenshot_2020-09-17_01-34-27.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/fa274b12-8ee7-41f7-94df-5d9aafc28ff2/Screenshot_2020-09-17_01-34-27.png)

### 드디어 설정다른값을 주고 하니 성공...

해당 와이파이 DEAUTH로 연결 안되고 똑같은 AP로 연결됨

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/0b6214c3-acb5-4d7b-95f2-4b20463c0dbf/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/0b6214c3-acb5-4d7b-95f2-4b20463c0dbf/Untitled.png)

- 사용자가 여기에 비밀번호를 입력하면....

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/329746da-680a-408d-8a92-8da712857ddc/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/329746da-680a-408d-8a92-8da712857ddc/Untitled.png)

### 성공!!

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/01f4b31d-f9eb-4fc5-b2ca-31264d907831/Screenshot_2020-09-17_01-39-57.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/01f4b31d-f9eb-4fc5-b2ca-31264d907831/Screenshot_2020-09-17_01-39-57.png)

### 비밀번호 얻기 성공

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5dfcf3b1-e3ac-42a9-8968-5e11c09a8989/Screenshot_2020-09-17_01-41-43.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5dfcf3b1-e3ac-42a9-8968-5e11c09a8989/Screenshot_2020-09-17_01-41-43.png)

Fluxion 원리

1. 선택한 해당 wifi(wpa, wpa2)의 정보를 얻어 해쉬값으로 저장.
2. 해당 wifi에 deauth attack
3. 얻은 정보를 바탕으로. [해당 wifi]로 보이는 AP생성
4. 사용자는 새로생긴 AP에 연결. 기존 AP 연결이 안되기 때문에. → 이때 사용자는 비밀번호 입력!!
5. Fluxion은 받은 비밀번호를 이용하여 기존 AP에 연결가능한지 확인.
6. 새로 얻은 비밀번호로 접속 가능하면 log파일로 자동 저장됨.  

→ 비밀번호 탈취 성공 !!!

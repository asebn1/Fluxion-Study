# Fluxion-Study
Fluxion : Wi-Fi password stealing



```bash
git clone https://github.com/FluxionNetwork/fluxion.git
```

```bash
cd fluxion
sudo ./fluxion.sh -i
```

- 패킷 잘 안잡힐 때
```bash
airmon-ng start fluxwl0
airmon-ng check kill
```
- 위 명령어 실행 후 하니 잘 잡힘

- virtualBox 에서 패킷 잡다보면 잡힐때도 있고 안잡힐때도 있어서 너무 시간 오래걸림. 한번 시도할때마다 재시도할때 많음.. 그래서 그냥 가상머신 말고 자체 칼리로 시도함

# Fluxion 원리

1. 선택한 해당 wifi(wpa, wpa2)의 정보를 얻어 해쉬값으로 저장.
2. 해당 wifi에 deauth attack
3. 얻은 정보를 바탕으로. [해당 wifi]로 보이는 AP생성
4. 사용자는 새로생긴 AP에 연결. 기존 AP 연결이 안되기 때문에. → 이때 사용자는 비밀번호 입력!!
5. Fluxion은 받은 비밀번호를 이용하여 기존 AP에 연결가능한지 확인.
6. 새로 얻은 비밀번호로 접속 가능하면 log파일로 자동 저장됨.  

→ 비밀번호 탈취 성공 !!!

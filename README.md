# simple_tgbot
파이썬을 활용한 텔레그램 봇. 본래는 Berachain bArtio 테스트넷에서의 아비트라지에 활용할 목적으로 만듦  
텔레그램 앱 상호작용 X. 단순 값 반복 출력

## main_public.py
- 단순히 원하는 특정 값을 반복해서 출력해주는 봇
- API_TOKEN에는 본인의 텔레그램 봇의 API token을 (텔레그램 봇 생성은 https://web.telegram.org/k/#@BotFather 참고할 것),  GROUP_CHAT_ID에는 본인의 봇이 들어가 있는 채널의 CHAT_ID(https://api.telegram.org/bot'봇Token값'/getUpdates 활용)를 기입하면 됨
- API_URL은 Etherscan API Endpoints(https://docs.etherscan.io/ 참고)를 활용하여 얻은 result를 단순 출력에 활용함.

## main_web3_public.py
- 특정 조건이 충족되었을 때 트랜잭션을 전송하는 봇
- API Endpoint 활용은 main_public.py와 동일함
- Web3 Provider URI는 본인이 트랜잭션을 보내고 싶은 체인의 RPC Node로 세팅, Transaction에서 역시 해당 체인의 Chain ID 사용

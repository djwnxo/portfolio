# **개발동기**
기본적인 디스코드 서버를 만들 때 여러 봇을 사용하여 필요한 기능을 충족해야했지만 하나의 봇으로 기능을 통일하고 싶었기 때문에 만들게 되었다.
# **선행 연구**
디스코드 개발자 포털로 관리자 권한을 가지고 있는 디스코드 봇을 생성 후 임의로 만든 테스트 서버에 추가했다. 
파이썬으로 디스코드 라이브러리를 불러와 디스코드 봇 토큰을 사용하여 봇을 실행 시킬 수 있는 방법, intents를 활용하여 봇을 실행 시킨 후 프로그램 해놓은 명령어를 작동시켜주는 방법에 대해 알게 되었다.
# **개발환경**
tool : VsCode, Discord
test : Discord
# **핵심코드**
디스코드 봇을 제작하는 과정에서 가장 중요하게 생각한 코드는 아래 코드로 정리할 수 있을 것 같다.
```
client = discord.Client(intents=discord.Intents.all())

async def main(): #cmd 클래스를 실행 시켜주는 main() 함수 호출

async def run_bot_and_main(): #client 명령어와 main() 함수를 하나의 함수로 정의

if __name__ == '__main__': #run_bot_and_main() 함수 호출

@client.event
async def on_ready(): #봇의 상태를 온라인으로 변경 시켜주고 상태설정을 설정할 수 있다.
```


# **느낀점 혹은 개선점**


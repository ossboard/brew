
# 

# brew 설치
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew install mas
mas install 497799835  # mas search xcode , 497799835  Xcode (14.0.1)
mas install 869223134  # mas search kakao , 869223134  카카오톡 (3.0.8)
mas install 1218085720 # mas search MotionPro , 1218085720  MotionPro Plus (2.0.2)

brew install chroma
brew install tomcat@9
brew install --cask oracle-jdk # 오라클 jdk 19이상
brew install --cask intellij-idea # 인텔리제이
brew install --cask github # 깃허브
brew install --cask sublime-text # 서브라임텍스트(text편집기)
brew install --cask microsoft-office # ms오피스
brew install --cask notion # 노션
brew install --cask visual-studio-code # VSC
brew install --cask gas-mask # hosts편집기
brew install --cask google-chrome # 구글크롬

```


# brewfile

```
cask "oracle-jdk"
cask "sublime-text"
cask "visual-studio-code"
mas "MotionPro Plus", id: 1218085720
ossboard@MacBook-Pro ~ % 

```

# Monterey에서 한글 shift+space
```
Monterey 출시 후 한/영 전환키가 Shift+Space키가 fn+Shift+Space키로 설정할 수 없음
(Xcode를 설치후)\
Finder -> (Cmd+Shift+G) -> ~/Library/Preferences/com.apple.symbolichotkeys.plist
xcode 로 열기 > 파일의 61번 > value > parameters > item 2 > '786432' -> '131072'로 변경하고, 리부팅
```

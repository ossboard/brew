
# 

# brew 설치
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew install mas
mas install 497799835  # mas search xcode , 497799835  Xcode (14.0.1)
mas search kakao , # mas search kakao , 869223134  카카오톡 (3.0.8)
mas search MotionPro , 1218085720  MotionPro Plus (2.0.2)

brew install chroma
brew install tomcat@9
brew install --cask oracle-jdk
brew install --cask intellij-idea
brew install --cask github
brew install --cask sublime-text
brew install --cask microsoft-office
brew install --cask notion
brew install --cask visual-studio-code
brew install --cask gas-mask


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

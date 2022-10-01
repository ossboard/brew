
# 

# brew 설치
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew install mas
mas install 497799835  # mas search xcode , 497799835  Xcode (14.0.1)
mas install 869223134  # mas search kakao , 869223134  카카오톡 (3.0.8)
mas install 1218085720 # mas search MotionPro , 1218085720  MotionPro Plus (2.0.2)

brew install tree
brew install htop
brew install git # 기본보다최신버전

brew install figlet # 놀기용
brew install lolcat # figlet와함께

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
brew install --cask alfred
brew install --cask iterm2
brew install --cask miniconda

brew install gromgit/fuse/sshfs-mac
https://github.com/osxfuse/sshfs/releases <-또는 직접pkg설치

# oh-my-zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
vi ~/.zshrc
---
#ZSH_THEME="robbyrussell"
ZSH_THEME="random"  #ZSH_THEME="agnoster"
...
ZSH_THEME_RANDOM_CANDIDATES=( "robbyrussell" "agnoster" )
---

*폴트설치
git clone https://github.com/powerline/fonts.git --depth=1
* 터미널설정 / Profiles / Font -> 'Inconsolate-dz for Powerline 11' 변경 
* Iterm2설정 / Profiles / Text / Font -> 
vi ~/.oh-my-zsh/themes/agnoster.zsh-theme 
-----
205 # Dir: current working directory
206 prompt_dir() {
207   #prompt_segment blue $CURRENT_FG '%~'
       prompt_segment 39d $CURRENT_FG '%~'
----


```



# 일괄설치 brewfile
```
#brewFile 생성 (새로 생성)
touch Brewfile

#brewFile 생성 (Mac에 설치된 항목들을 BrewFile로 저장한 채로 )
brew bundle dump

#brewFile 덮어쓰기
brew bundle -f dump

#brewFile 확인
cat Brewfile
```

# Monterey에서 한글 shift+space
```
Monterey 출시 후 한/영 전환키가 Shift+Space키가 fn+Shift+Space키로 설정할 수 없음
(Xcode를 설치후)\
Finder -> (Cmd+Shift+G) -> ~/Library/Preferences/com.apple.symbolichotkeys.plist
xcode 로 열기 > 파일의 61번 > value > parameters > item 2 > '786432' -> '131072'로 변경하고, 리부팅
```

# figlet
``` 
cd /usr/local/share/figlet/fonts/ && ls *.flf
figlet -f slant -c ossboard
figlet -f slant -c Konan Tech
figlet -f speed -c Konan Tech
figlet -f slant -c Konan Tech | lolcat

```

# 기타정보
``` 
Rosetta <-- Rosetta는 M1과 같이 ARM 기반의 칩을 사용하는 환경에서 x86 아키텍쳐를 사용하여 디자인된 Intel 기반 칩용 앱을 실행

```
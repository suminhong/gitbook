---
description: 맥 초기 세팅 시 설치할 것들
---

# Install

### 1. Homebrew

{% code fullWidth="true" %}
```bash
# brew 다운로드
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# 경로 추가
echo 'export PATH=/opt/homebrew/bin:$PATH' >> ~/.zshrc
source ~/.zshrc

# 설치 확인
brew --version
```
{% endcode %}

### 2. ishot

{% embed url="https://apps.apple.com/kr/app/ishot-screenshot-recording-ocr/id1485844094?mt=12" %}

사용해본 캡쳐 툴 중 제일 좋음.

`option + a` 로 캡쳐

### 3. spectacle

[https://github.com/eczarny/spectacle/releases/download/1.2/Spectacle+1.2.zip](https://github.com/eczarny/spectacle/releases/download/1.2/Spectacle+1.2.zip)

화면 분할 앱. 무료인데 유료만큼 함 (현재는 deprecate되었는데 위 링크로 다운 가능. 보통은 rectangle로 넘어감)

### 4. brew로 각종 도구 설치

```bash
brew install iterm2 zsh awscli weaveworks/tap/eksctl gjbae1212/gossm/gossm saml2aws tfenv terraform-docs pre-commit kubectl kubectx k9s helm git gh wget telnet mysql python watch poetry iproute2mac lsd
brew install --cask docker openlens rectangle
```

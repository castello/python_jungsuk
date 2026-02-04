# 파이썬 수업준비

## [MacOS]
 1-1. homebrew설치
 1-2. x-code설치되었는지 확인
 1-3. 깃 설치
> brew install git

1-4. penv설치
brew update
brew install pyenv
echo 'export PYENV_ROOT="$HOME/-pyenv"' >> ~/.zshrc
echo '[[-d $PYENV_ROOT/bin ]] && export PATH="$PYENV_ROOT/bin: $PATH"' > ~/. zshrc
echo 'eval "$(pyenv init -)"' >> ~/.zshrc

exec "$SHELL"
터미널 재시작

1-5 python설치
>pyenv install 3.11
>pyenv global 3.11
>exec zsh
> python --version


## [윈도우즈]
1-1 깃 설치
1-2 pyenv설치 - 여러 버전의 파이썬 사용가능

> git clone https: //github.com/pyenv-win/pyenv-win.git "$env: USERPROFILE\ - pyenv"

PS C: \Users\Administrator> [System. Environment]:: SetEnvironmentVariable('PYENV',
$env: USERPROFILE + "\.pyenv\pyenv-win\", "User")

PS C: \Users\Administrator> [System. Environment]::SetEnvironmentVariable('PYENV_ROOT' ,

$env: USERPROFILE + "\. pyenv\pyenv-win\", "User")

PS C: \Users\Administrator> [System. Environment]:: SetEnvironmentVariable('PYENV_HOME',

$env: USERPROFILE + "\. pyenv\pyenv-win\", "User")

PS C:\Users \Administrator> [System. Environment]:: SetEnvironmentVariable( 'PATH', $env: USERPROFILE + "I-pyenv\pyenv-win\bin;" + $env: USERPROFILE + "\.pyenv\pyenv-win\
shims;" + [System. Environment]:: GetEnvironmentVariable('PATH', "User"), "User")


1-3 python설치 using pyenv
> pyenv install 3.11

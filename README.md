## Firebaseでの開発方法

1. Nodejsが必要
   1. そのために[NVM](https://github.com/nvm-sh/nvm)をインストールするべき
      1. sudo apt install nodejs でも入るがグローバルインストールなどでパーミッションの問題に当たるのでNVMで入れるのを推奨
   2. インストール方法
      1. `curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.34.0/install.sh | bash`
      2. 使っているshellに応じて
         1. bashを使っている人は  
          ~/.bashrc or ~/.bash_profile
         1. zshを使っているいる人は  
        ~/.zshrc ~/.zprofile
      3. どちらかに下記を記載する  
            ```
            export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
            [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm
            [ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion" # This loads nvm bash_completion
            ```
      4. 記載したら`nvm install --lts`でnodejsとnpmの長期安定版をインストールする
      5. これはnvmを構築したユーザーにしか適用されない



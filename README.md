# ansible-lesson

●Docker内でAnsibleの勉強をしよう

https://qiita.com/comefigo/items/34209c391962ab0c8f1b

あたりを参考にしつつ、Ansible でDockerの上のサーバをプロビジョニングする為の環境を作製。

また、

●2017年版 SSH公開鍵認証で使用する秘密鍵ペアの作り方

https://qiita.com/wnoguchi/items/a72a042bb8159c35d056

を参考に、sshキーは新たにEd25519で以下のように作り直した。

ssh-keygen -t ed25519 -P "" -C "ansible lesson" -f ansible_ed25519
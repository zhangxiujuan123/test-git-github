## 个人开发项目用git
第一步 : 在需要git 管理的文件夹下打开git base here 
第二步：在git中进行项目管理的初始化 git init
第三步：在git中创建自己的项目文件
第四步：通过git add * 将所有的项目文件添加进去临时区域内
第五步：通过git commit -m 操作说明  将临时区域内的项目推送到本地的仓库上去
第六步：对项目进行修改之后,可以先看看修改了哪些东西，git diff 
第七步：确认完修改之后，可以通过git commit -a -m 操作说明 来进行上传了.
第八步：如果需要切换版本，只需要通过git reflog 查看下自己的操作历史，然后通过git reset 
--hard 版本号 就可以自由的切换不同的状态了。
第九步: 如需删除文件，使用git rm 文件名 来进行删除,然后通过git commit -a -m 提交
第十步:如果发生在本地误删的情况，可以直接使用git checkout 把临时区域的内容拉到本地



输入git log 到END时，按q键

## 合作开发
1.创建本地ssh密钥，作用：告诉远程仓库 是你自己推送的消息
$ ssh-keygen -t rsa -C "emailAddress"

查看生成的公钥
$ cat ~/.ssh/id_rsa.pub

ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCv30/TiP5IoPE5TEmk5Dk+xlQkz5GGBreL/mX9DPUYY63sWuPNQu65BuI1LzZvGaEsLvEr5MlvUeYkfGGdDN091BygYMsP7oc2ZJiaEdv9Z68xhfuKNsYQURFamDvH3dV/Q0M7ttyAqXZx3R9DauS3mRjApE5p67eWbXJGLMtG58/eFWtyJPe0PluxrDOoAGhNiwJeFBlXE1gkhNsYCSiS5FWBOy906gdpr/Dx14h4608FX+NRR5Gcnbt8c4kKQZ2L++Gfibk3IKszZOhDhO5N/1GApwy2nBTB4c6bQPZdvpRtORYEjDI821vOEwJylBPRZqR4lk+MNjz9aBf4myQiu6kKPCnxjXKv2HkFsk6Znw8opaH/v7KaYSEKa88CWg0I4v0PmuijtLbYLEv3BCXq1pVdHcJVfqLXYpNgyI40ue58I8VloSLQRvREGjcgk4oz+djIuzEX3K2uk6BOVG8vminQZTqp1aYkITDrEhmOSCaOLW0IE9dxZJRtnAqe1Yk= 1982708792@qq.com

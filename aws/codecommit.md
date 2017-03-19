# codecommit の使い方メモ
2017.3.18 記

# linux

aws-cli のインストール
```
pip install awscli
```

```
$aws configure --profile CodeCommitProfile

AWS Access Key ID [None]: 
AWS Secret Access Key [None]: 
Default region name [None]: us-east-1 
Default output format [None]: 
```

```
$git config --global credential.helper '!aws --profile CodeCommitProfile codecommit credential-helper $@'
$git config --global credential.UseHttpPath true
```

 利用
 ```
 git config --global credential.helper "!aws codecommit credential-helper $@"

git config --global credential.UseHttpPath true
  
git clone https://git-codecommit.us-east-1.amazonaws.com/v1/repos/sangyonci

 ```


miyamoto-masanao

AKIAJDMVEVSFLM4JHUIA
EbOODZ6kljQLRBXoWi1u7vb0Qr+U4u798X8ABa2k

# windows

### 初めに git for windows をインストールする。


### AWS Cli のインストール

http://docs.aws.amazon.com/cli/latest/userguide/awscli-install-windows.html

### AWS Tools のインストール

AWS Tools for PowerShell　をダウンロード・インストール

https://aws.amazon.com/jp/tools/

### AWS設定

```
aws configure
AWS Access Key ID [None]: AKIAJDMVEVSFLM4JHUIA
AWS Secret Access Key [None]: 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
Default region name [None]: us-east-1
Default output format [None]:

```

c:\Program Files (x86)\AWS Tools\CodeCommit

## 参考にしたURL

http://qiita.com/toshihirock/items/5f748e785fdd3b463b6a


http://docs.aws.amazon.com/codecommit/latest/userguide/setting-up-https-windows.html

https://www.slideshare.net/AmazonWebServicesJapan/aws-black-belt-tech-2015-aws-codecommit-aws-codepipeline-aws-codedeploy

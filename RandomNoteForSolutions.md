# Random Note For Solutions

## 23.10.10
#### When debugging in vs code, it may shows like this.

![pic](pics/1.png)

This is because the folders' names must not be Chinese, MinGw does not support Chinese path.


#### `<iostream.h>` and `void main` are not supported now, we use  

    #include<iostream>
    using namespace std;

and `int main`

## 23.10.12
### Git报错解决：fatal: unable to access ‘https://github.com/…’: OpenSSL SSL_read: Connection was reset, errno 10054

`一般是这是因为服务器的SSL证书没有经过第三方机构的签署，所以才报错`
参考网上解决办法：解除ssl验证后，再次git即可

`git config --global http.sslVerify "false"`
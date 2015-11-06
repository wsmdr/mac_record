# Mac - Homebrew - Nginx - Php - Mysql

## 安装Homebrew

``` ruby
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

``` 
xcode-select --install
```

**brew install nginx**

> nginx默认8080端口 
> 
> 可在 /usr/local/etc/nginx/nginx.conf 文件修改

**brew install mysql**

**brew install homebrew/php/php56**

> 由于Mac自带php版本  安装完之后需要添加php56到PATH中 
> 
> export PATH="$(brew --prefix homebrew/php/php56)/bin:$PATH"

## 常用php扩展

* brew install php56-mycrypt


* brew install php56-memcache
  
* brew install php56-memcached
  
  * brew link --force zlib
    
  * 未安装zlib
    
    * ``` 
      brew tap homebrew/dupes
      brew install zlib
      ```


* brew install php56-phalcon


* brew install php56-redis


* brew install php56-swoole


* brew install php56-xdebug

## brew cask 安装 Mac程序

``` 
brew install caskroom/cask/brew-cask
```
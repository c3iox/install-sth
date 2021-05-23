# node&npm

## nodejs(with npm) 

使用包仓库模式安装node，详见 [GITHUB centos repo](https://github.com/nodesource/distributions)

### centos(tlinux)

1. 下载  install.sh 
	```bash
	wget https://rpm.nodesource.com/setup_16.x -O install.sh
	```

2. 编辑 install.sh

    替换DISTRO_PKG值（默认的rpm -q --whatprovides centos-release返回的是tlinux版本）

    ```bash
    DISTRO_PKG="centos-release-7-2.2003.0.el7.centos.x86_64"
    ```

3. 执行 install.sh

    ```bash
    bash install.sh
    ```

4. 替换 npm源

    更换掉网络不稳定的默认源，换成高效稳定的国内源

    ```bash
    npm config set registry https://registry.npm.taobao.org
    ```

    

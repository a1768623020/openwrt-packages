# Docker Manager interface for LuCI

## ������ LuCI �� Docker ������
���ڹ��� Docker �������������磬�������Դ� Docker �� Openwrtϵͳ�������� Docker �е� openwrt �� [LuCI-in-docker](https://github.com/lisaac/luci-in-docker).

### Depends/����
- luci-lib-json
- [luci-lib-docker](https://github.com/lisaac/luci-lib-docker)

### Compile/����
```bash
./scripts/feeds update luci-lib-json
./scripts/feeds install luci-lib-json
git clone https://github.com/lisaac/luci-lib-docker.git package/luci-lib-docker
git clone https://github.com/lisaac/luci-app-dockerman.git package/luci-app-dockerman

#compile package only
make package/luci-lib-json/compile V=99
make package/luci-lib-docker/compile v=99
make package/luci-app-dockerman/compile v=99

#compile
make menuconfig
#choose Utilities  ---> <*> docker-ce....................................... Docker Community Edition
#choose Kernel features for Docker which you want
#choose LuCI ---> 3. Applications  ---> <*> luci-app-dockerman..... Docker Manager interface for LuCI ----> save
make V=99
```

### Download /����
- [ipk file](https://github.com/lisaac/luci-app-dockerman/releases)

### Screenshot/��ͼ
- Containers
![](https://raw.githubusercontent.com/lisaac/luci-app-dockerman/master/doc/containers.png)
- Container Info
![](https://raw.githubusercontent.com/lisaac/luci-app-dockerman/master/doc/container_info.png)
- Container Edit
![](https://raw.githubusercontent.com/lisaac/luci-app-dockerman/master/doc/container_edit.png)
- Container Stats
![](https://raw.githubusercontent.com/lisaac/luci-app-dockerman/master/doc/container_stats.png)
- Container Logs
![](https://raw.githubusercontent.com/lisaac/luci-app-dockerman/master/doc/container_logs.png)
- New Container
![](https://raw.githubusercontent.com/lisaac/luci-app-dockerman/master/doc/new_container.png)
- Images
![](https://raw.githubusercontent.com/lisaac/luci-app-dockerman/master/doc/images.png)
- Networks
![](https://raw.githubusercontent.com/lisaac/luci-app-dockerman/master/doc/networks.png)
- New Network
![](https://raw.githubusercontent.com/lisaac/luci-app-dockerman/master/doc/new_network.png)

### Thanks
- Chinese translation by [401626436](https://www.right.com.cn/forum/space-uid-382335.html)

### TODO:
- images: edit_tag / import
- new network: analyze command line string
- container: download & upload files

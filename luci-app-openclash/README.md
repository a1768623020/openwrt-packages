<h1 align="center">
  <img src="https://github.com/Dreamacro/clash/raw/master/docs/logo.png" alt="Clash" width="200">
  <br>OpenClash<br>

</h1>

  <p align="center">
	<a target="_blank" href="https://github.com/Dreamacro/clash/releases/tag/v0.17.0">
    <img src="https://img.shields.io/badge/Clash-v0.17.0-blue.svg">
  </a>
  <a target="_blank" href="https://github.com/vernesong/OpenClash/tree/v0.36.5-beta">
    <img src="https://img.shields.io/badge/source code-v0.36.5--beta-green.svg">
  </a>
  <a target="_blank" href="https://github.com/vernesong/OpenClash/releases/tag/v0.36.5-beta">
    <img src="https://img.shields.io/badge/New Release-v0.36.5--beta-orange.svg">
  </a>
  </p>
  

<p align="center">
�������һ���������� OpenWrt �ϵ�<a href="https://github.com/Dreamacro/clash" target="_blank"> Clash </a>�ͻ���
</p>
<p align="center">
���� Shadowsocks��Vmess��Snell ��Э�飬�������Ĺ�������ʵ�ֲ��Դ���
</p>
<p align="center">
- ��л<a href="https://github.com/frainzy1477" target="_blank"> frainzy1477 </a>�����������<a href="https://github.com/frainzy1477/luci-app-clash" target="_blank"> Luci For Clash </a>���ж��ο��� -
</p>

ʹ���ֲ�
---


* [Wiki](https://github.com/vernesong/OpenClash/wiki)


���ص�ַ
---


* IPK [ǰ������](https://github.com/vernesong/OpenClash/releases)


����
---

* luci
* luci-base
* iptables
* dnsmasq-full
* coreutils
* coreutils-nohup
* bash
* curl
* jsonfilter
* ca-certificates
* kmod-tun(TUNģʽ)
* luci-compat(Luci-19.07)


����
---


�� OpenWrt �� [SDK](http://wiki.openwrt.org/doc/howto/obtain.firmware.sdk) ����
```bash
# ��ѹ���غõ� SDK
tar xjf OpenWrt-SDK-ar71xx-for-linux-x86_64-gcc-4.8-linaro_uClibc-0.9.33.2.tar.bz2
cd OpenWrt-SDK-ar71xx-*

# Clone ��Ŀ
mkdir package/luci-app-openclash
cd package/luci-app-openclash
git init
git remote add -f origin https://github.com/vernesong/OpenClash.git
git config core.sparsecheckout true
echo "luci-app-openclash" >> .git/info/sparse-checkout
git pull origin master
git branch --set-upstream-to=origin/master master

# ���� po2lmo (�����po2lmo������)
pushd package/luci-app-openclash/luci-app-openclash/tools/po2lmo
make && sudo make install
popd

# ѡ��Ҫ����İ� LuCI -> Applications -> luci-app-openclash
make menuconfig

# ��ʼ����
make package/luci-app-openclash/luci-app-openclash/compile V=99

# ��Ҳ����ֱ�ӿ��� `luci-app-openclash` �ļ��������� `OpenWrt` ��Ŀ�� `Package` Ŀ¼����̼�����
```


���
---


* [MIT License](https://github.com/vernesong/OpenClash/blob/master/LICENSE)
* �ں� [clash](https://github.com/Dreamacro/clash) by [Dreamacro](https://github.com/Dreamacro)
* ����Ŀ������� [Luci For Clash](https://github.com/frainzy1477/luci-app-clash) by [frainzy1477](https://github.com/frainzy1477)
* GEOIP���ݿ� [GeoLite2](https://dev.maxmind.com/geoip/geoip2/geolite2/) by [MaxMind](https://www.maxmind.com)
* IP��� [MyIP](https://github.com/SukkaW/MyIP) by [SukkaW](https://github.com/SukkaW)
* ������� [clash-dashboard](https://github.com/Dreamacro/clash-dashboard) by [Dreamacro](https://github.com/Dreamacro)
* ������� [yacd](https://github.com/haishanh/yacd) by [haishanh](https://github.com/haishanh)
* lhie1���� [lhie1-Rules](https://github.com/lhie1/Rules) by [lhie1](https://github.com/lhie1)
* ConnersHua���� [ConnersHua-Rules](https://github.com/ConnersHua/Profiles/tree/master) by [ConnersHua](https://github.com/ConnersHua)
* ��Ϸ���� [SSTap-Rule](https://github.com/FQrabbit/SSTap-Rule) by [FQrabbit](https://github.com/FQrabbit)
* ����ת��API [Api_Constructor](https://fndroid.github.io/api_constructor/) by [Fndroid](https://github.com/Fndroid)


�����ߺȱ�����
---

* ���ر�-BTC
<p align="left">
    <img width="300" src="https://github.com/vernesong/OpenClash/raw/master/img/BTC-Wallet.png">
</p>

* ��̫��-ETH
<p align="left">
    <img width="300" src="https://github.com/vernesong/OpenClash/raw/master/img/ETH-Wallet.png">
</p>


Ԥ��
---


* ����״̬
<p align="center">
    <img src="https://github.com/vernesong/OpenClash/raw/master/img/state.png">
</p>

* ȫ������
<p align="center">
    <img src="https://github.com/vernesong/OpenClash/raw/master/img/settings.png">
</p>

* ������&������
<p align="center">
    <img src="https://github.com/vernesong/OpenClash/raw/master/img/servers.png">
</p>

* ��Ϸ����&������
<p align="center">
    <img src="https://github.com/vernesong/OpenClash/raw/master/img/game-settings.png">
</p>

* �����ļ�����
<p align="center">
    <img src="https://github.com/vernesong/OpenClash/raw/master/img/config-subscribe.png">
</p>

* �����ļ�����
<p align="center">
    <img src="https://github.com/vernesong/OpenClash/raw/master/img/config.png">
</p>

* ������־
<p align="center">
    <img src="https://github.com/vernesong/OpenClash/raw/master/img/log.png">
</p>

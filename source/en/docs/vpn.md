title: VPN 使用手冊
---

## PPTP
To be continue...


## OpenVPN

### Windows
To be continue...

### MacOS
This tutorial consists of two sections, choose either one as you please.
* [Tunnelblick](#tunnelblick) ==for beginner==
* [Terminal](#terminal) ==for advanced user ~~and good CS student~~ :smiley:~==

#### Tunnelblick

0. Visit [Tunnelblick Website](https://tunnelblick.net). Click on the green arrow icon says "Download Latest Stable Release" on the left.
![](https://www2.cs.ccu.edu.tw/~cchuo102u/tmp/openvpn/tunnelblick_0.png)

1. When warning window pops, click on "Open".
![](https://www2.cs.ccu.edu.tw/~cchuo102u/tmp/openvpn/tunnelblick_1.png)

2. Open the dmg file downloaded. Double-click on the Tunnelblick icon.
![](https://www2.cs.ccu.edu.tw/~cchuo102u/tmp/openvpn/tunnelblick_2.png)

3. Type your username on mac and password to allow installation.
![](https://www2.cs.ccu.edu.tw/~cchuo102u/tmp/openvpn/tunnelblick_3.png)

4. After installation, drag and drop the [CCUCS VPN Config](https://vpn.cs.ccu.edu.tw/clients/ccucsie.ovpn) to the "Configuration" column on the left.
![](https://www2.cs.ccu.edu.tw/~cchuo102u/tmp/openvpn/tunnelblick_4.png)

5. Click on "Coonect" on the bottom right cornner (as shown above), OR click on Tunnelblick icon next to Spotlight (as shown below) and click on "Connect ccucsie".
![](https://www2.cs.ccu.edu.tw/~cchuo102u/tmp/openvpn/tunnelblick_5-1.png)
![](https://www2.cs.ccu.edu.tw/~cchuo102u/tmp/openvpn/tunnelblick_5-2.png)

6. Login with your username on CCUCS workstation and password.
![](https://www2.cs.ccu.edu.tw/~cchuo102u/tmp/openvpn/tunnelblick_6.png)

7. The message "ccucsie Connected" indicated that VPN connection is successfully created.
![](https://www2.cs.ccu.edu.tw/~cchuo102u/tmp/openvpn/tunnelblick_7.png)

#### Terminal

0. Install package management tool [Homebrew](https://brew.sh).
```
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
> Q: What does homebrew do?
> A: Homebrew installs the stuff you need that Apple didn’t.[name=#homebrew][color=brown]

1. Install OpenVPN with Homebrew.
```
$ brew install openvpn
```

2. Since `openvpn` being placed under `/usr/loca/sbin/`, add the following line to `~/.bashrc` for it was not in `PATH` by default. Then, `source ~/.bashrc`.
```
export PATH=/usr/local/sbin:$PATH
```

3. Connect with `openvpn`. ([Download OpenVPN Config](https://vpn.cs.ccu.edu.tw/clients/ccucsie.ovpn))
```
$ sudo openvpn /path/to/config/ccucsie.ovpn
```
![](https://www2.cs.ccu.edu.tw/~cchuo102u/tmp/openvpn/terminal_3.png)

4. The message "Initialization Sequence Completed" indicated that VPN connection is successfully created.
```
Sun Nov 12 11:17:53 2017 Initialization Sequence Completed
```

5. (Optional) Since the password may be cached in memory, please consider using option `auth-nocache` to enhance security.
```
WARNING: this configuration may cache passwords in memory -- use the auth-nocache option to prevent this
```


## Bug Report
When shit happens, please contact CS Computer Centre.
- [About US](/about/)

<i class="fa fa-edit fa-fw"></i> Last Edited: _2018/07/08 by setsal_, contributed by _silenttulips_

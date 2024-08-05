# vps-bench
Bench Script based on https://github.com/teddysun/across/blob/master/bench.sh

## Version: 2024v1

*Sample run - copy and paste to Terminal command without dollar sign:*

`$ wget -qO- jurkiewicz.tech/vps-bench.sh | bash`

---

## Changes made:

* changing test of ip to non-chinese servers: `google` and `ipinfo`
* getting list of nearest Speedtest servers, and extract 3 best
* checking OS:
    * `/etc/redhat-release`
    * `/etc/os-release`
    * `/etc/lsb-release`
    * if non of above exist, script reports "Not supported OS - EXIT!" and do `_exit`

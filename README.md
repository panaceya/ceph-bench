# ceph-bench
Tool for benchmark Ceph

# Install pre-requrements

### CentOS
`yum install python-configparser python-monotonic`
### Debian/Ubuntu
* for Python2 `apt install python-configparser python-monotonic`
* for Python3 `apt install python3-rados`

# Prepare

```
cd ceph-bench
ceph auth export client.admin -o keyring.conf
ceph osd pool set single size 1
ceph osd pool create single 1 1
```

# Run
* for Python2 `python2 main.py`
* for Python3 `python3 main.py`

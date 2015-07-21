# RAVE UP advertising

- Repository https://github.com/raveupadvertising/raveupadvertising.github.io
- Website for www.raveupadvertising.com

#### Plan

- [x] github raveupadvertising.com
- [x] justhost CNAME
- [ ] transfer raveup

#### Config

**Before**

```sh
dig raveupadvertising.com +nostats +nocomments +nocmd

; <<>> DiG 9.8.3-P1 <<>> raveupadvertising.com +nostats +nocomments +nocmd
;; global options: +cmd
;raveupadvertising.com.		IN	A
raveupadvertising.com.	14399	IN	A	173.254.28.38
```

**After**

```sh
dig raveupadvertising.com +nostats +nocomments +nocmd

; <<>> DiG 9.8.3-P1 <<>> raveupadvertising.com +nostats +nocomments +nocmd
;; global options: +cmd
;raveupadvertising.com.		IN	A
raveupadvertising.com.	446	IN	A	192.30.252.154
raveupadvertising.com.	446	IN	A	192.30.252.153
```

**Stack Overflow http://stackoverflow.com/a/23375423**

```
@        A        192.30.252.153
@        A        192.30.252.154
www      CNAME    your_github_username.github.io.
```

#### Working DNS

```
host    record         points to
-------------------------------------
A       localhost      127.0.0.1
A       @              192.30.252.153
A       @              192.30.252.154
A       autoconfig     192.30.252.153
A       autodiscover   192.30.252.153
CNAME   www            raveupadvertising.github.io
```

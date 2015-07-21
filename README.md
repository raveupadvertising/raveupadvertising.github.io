# advertising
Website for www.raveupadvertising.com

#### Plan

- [x] github raveupadvertising.com
- [ ] justhost CNAME
- [ ] transfer raveup

```sh
dig raveupadvertising.com +nostats +nocomments +nocmd

; <<>> DiG 9.8.3-P1 <<>> raveupadvertising.com +nostats +nocomments +nocmd
;; global options: +cmd
;raveupadvertising.com.		IN	A
raveupadvertising.com.	14399	IN	A	173.254.28.38
```

**Create A records that resolve to the following IP addresses:**

- 192.30.252.153
- 192.30.252.154

**Stack Overflow http://stackoverflow.com/a/23375423**

```
@        A        192.30.252.153
@        A        192.30.252.154
www      CNAME    your_github_username.github.io.
```

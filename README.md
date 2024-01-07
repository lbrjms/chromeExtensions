# chromeExtensions


```
// timeout=prompt("Set timeout (Second):");
timeout = 1;
count=0
current=location.href;
setTimeout('reload()',1000*timeout);
function reload(){
setTimeout('reload()',1000*timeout);
count++;
console.log('每（'+timeout+'）秒自动刷新,刷新次数：'+count);
fr4me='<frameset cols=\'*\'>\n<frame src=\''+current+'\'/>';
fr4me+='</frameset>';
with(document){write(fr4me);void(close())};
}
```

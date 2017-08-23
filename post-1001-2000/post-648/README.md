# #純靠北工程師648


假如停電是機率問題...


```
test $(expr $(od -vAn -N4 -tu4 < /dev/urandom) % 2) -eq 0 && echo "the power will outage" || echo "the power won't outage"
```

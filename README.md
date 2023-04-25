# turingpi




```bash

date -s @"$(curl -s "http://worldtimeapi.org/api/timezone/Asia/Seoul" | \
sed -n 's/.*"unixtime":\([0-9]*\).*/\1/p')"

hwclock --systohc
```

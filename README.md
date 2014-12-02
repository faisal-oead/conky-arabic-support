التنصيب
====================
ضع الملف في مجلد المنزل<br>
~/.conkyar/<br>

الإستخدام
====================
افتح الملف (.conkyrc)<br>

ضع هذي الأسطر الضرورية لدعم اللغة <br>
```
own_window_argb_visual yes
own_window_argb_value 255
override_utf8_locale yes
```
ضع هذا الامر في كل مره تريد الكتابة بالعربية<br>
${font arial:pixelsize=40}${alignc} ${exec  python2 ~/.conkyar/rtl.py "بسم الله الرحمن الرحيم"} ${font}<br>

![screenshot from 2014-12-02 16 01 04](https://cloud.githubusercontent.com/assets/7253063/5263727/8737b810-7a45-11e4-832e-eaa41a98ed87.png)


مثال
=====================
```
alignment top_middle
background yes
border_margin 5
border_width 5
default_color 000000
double_buffer yes
draw_borders no
draw_outline no
draw_shades no
gap_x 0
gap_y 80
maximum_width 1700
minimum_size 500 300
no_buffers yes
override_utf8_locale yes
own_window yes
own_window_title conky
own_window_hints undecorated,below,sticky,skip_taskbar,skip_pager
own_window_transparent yes
own_window_type normal 	## normal /override /desktop
text_buffer_size 8000
total_run_times 0
update_interval 1
uppercase no
use_xft yes
xftalpha 1
xftfont Freesans:pixelsize=9
own_window_argb_visual yes
own_window_argb_value 255

TEXT



${font arial:pixelsize=64}${alignc} ${exec  python2 ~/dev/python/rtl.py "بسم الله الرحمن الرحيم"} ${font}

${font arial:pixelsize=34}${alignc} ${exec  python2 ~/dev/python/rtl.py " إظافة دعم اللغة العربية في الكونكي "} ${font}




${font arial:pixelsize=24}${alignc}  ${mem} ${exec  python2 ~/dev/python/rtl.py " الرام : "} ${font}

${font arial:pixelsize=24}${alignc} ${upspeed eth0} ${exec  python2 ~/dev/python/rtl.py "  الشبكة صادر : "} ${font}
${font arial:pixelsize=24}${alignc}  ${downspeed eth0}  ${exec  python2 ~/dev/python/rtl.py " الشبكة تحميل : "} ${font}

${font arial:pixelsize=24}${alignc} %  ${cpu cpu0}  ${exec  python2 ~/dev/python/rtl.py " المعالج الأول    :  "} ${font}
${font arial:pixelsize=24}${alignc} %  ${cpu cpu1}  ${exec  python2 ~/dev/python/rtl.py "  المعالج الثاني  :  "} ${font}
${font arial:pixelsize=24}${alignc} %  ${cpu cpu2}  ${exec  python2 ~/dev/python/rtl.py "  المعالج الثالث :"} ${font}
${font arial:pixelsize=24}${alignc} %  ${cpu cpu3}  ${exec  python2 ~/dev/python/rtl.py "  المعالج الرابع :"} ${font}
```

لتواصل 
====================
https://www.facebook.com/faisal.sa13 <br>

شكر خاص 
====================
https://github.com/mpcabd/python-arabic-reshaper <br>

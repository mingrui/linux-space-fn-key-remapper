# linux-space-fn-key-remapper
turn space + h j k l => left, down, up, right
turn spacebar to a vim navigation fn key

Install this:

https://github.com/r0adrunner/Space2Ctrl

Now pressing space will register ctrl

Install xbindkeys xvkbd xbinkeys-config:

https://askubuntu.com/questions/834650/remap-a-key-combination-to-another-combination-e-g-superctrlshiftj-ctrl

follow these two guides to bind keys:

http://xahlee.info/linux/linux_xbindkeys_tutorial.htmlasdfasd

http://t-sato.in.coocan.jp/xvkbd/xvkbd-text.html

this is what my ~/.xbindkeysrc looks like:

```
"xvkbd -xsendevent -text "\[Left]""
    m:0x14 + c:43
    Control+Mod2 + h 

"xvkbd -xsendevent -text "\[Down]""
    m:0x14 + c:44
    Control+Mod2 + j 

"xvkbd -xsendevent -text "\[Up]""
    m:0x14 + c:45
    Control+Mod2 + k 

"xvkbd -xsendevent -text "\[Right]""
    m:0x14 + c:46
    Control+Mod2 + l 
```

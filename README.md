안녕하세요!

```
export MOZ_ENABLE_WAYLAND=1
export GDK_BACKEND=wayland

export IMSETTINGS_INTEGRATE_DESKTOP=yes
export IMSETTINGS_MODULE=fcitx5
export INPUT_METHOD=fcitx5
export GTK_IM_MODULE=fcitx5
export QT_IM_MODULE=fcitx5
export XMODIFIERS=@im=fcitx5
```


설정파일

~/.config/fcitx5/profile:
```
[Groups/0]
# Group Name
Name=Default
# Layout
Default Layout=kr-kr104
# Default Input Method
DefaultIM=hangul

[Groups/0/Items/0]
# Name
Name=keyboard-us
# Layout
Layout=

[Groups/0/Items/1]
# Name
Name=hangul
# Layout
Layout=

[GroupOrder]
0=Default
```

.config/fcitx5/conf/hangul.conf:

```
# Keyboard Layout
Keyboard=Dubeolsik
# Auto Reorder
AutoReorder=True
# Word Commit
WordCommit=False
# Hanja Mode
HanjaMode=False

[HanjaModeToggleKey]
0=Hangul_Hanja
1=F9

[PrevPage]
0=Up

[NextPage]
0=Down

[PrevCandidate]
0=Shift+Tab

[NextCandidate]
0=Tab

```

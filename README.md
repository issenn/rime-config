# rime-config

Rime 的 log 文件地址：

-【中州韻】 `/tmp/rime.ibus.*`

-【小狼毫】 `%TEMP%\rime.weasel.*`

-【鼠鬚管】 `$TMPDIR/rime.squirrel.*`

```sh
git clone https://github.com/rime/plum.git "${XDG_DATA_HOME:-${HOME}/.local/share}/Rime/plum"
bash "${XDG_DATA_HOME:-${HOME}/.local/share}/Rime/plum/rime-install" "double-pinyin"
bash "${XDG_DATA_HOME:-${HOME}/.local/share}/Rime/plum/rime-install" "terra-pinyin"
bash "${XDG_DATA_HOME:-${HOME}/.local/share}/Rime/plum/rime-install" "biopolyhedron/rime-jap-poly"
bash "${XDG_DATA_HOME:-${HOME}/.local/share}/Rime/plum/rime-install" "lotem/rime-kana"
bash "${XDG_DATA_HOME:-${HOME}/.local/share}/Rime/plum/rime-install" "Selaube/rime-jp_sela"
bash "${XDG_DATA_HOME:-${HOME}/.local/share}/Rime/plum/rime-install" "m13253/rime-nihongo-romaji"
bash "${XDG_DATA_HOME:-${HOME}/.local/share}/Rime/plum/rime-install" "sgalal/rime-kunyomi"
bash "${XDG_DATA_HOME:-${HOME}/.local/share}/Rime/plum/rime-install" "issenn/rime-config@master/brglng-packages.conf"
```

sys符号编码、补充简码

top置顶词库，当用户词和系统词重码，且需要用户词居前时设置

user用户词库，日常使用用户词添加到此文件

build文件夹内为码表文件

```sh
tail -f ${TMPDIR}rime.squirrel.*INFO*
tail -f ${TMPDIR}rime.squirrel.*WARNING*
tail -f ${TMPDIR}rime.squirrel.*ERROR*
```

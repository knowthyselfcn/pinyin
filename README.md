Lua 汉字转拼音的lib

参考 cyrilis/lua-pinyin lib，那个lib无法正常工作。没办法，只能自己改了。

bit.lua lib从 https://raw.githubusercontent.com/gourytch/freeminer_mods/master/coloured_signs/bit.lua获取的，无法在Lua5.1上正常工作，已做修改。
data 文件从hotoo/pinyin lib中获取的，由js数组修改为lua table。

使用方式：
local pinyin = require("pinyin.pinyin"):new()
pinyin:slugify( "这是一个中文字符串")
-- zhe-shi-yi-ge-zhong-wen-zi-fu-chuan

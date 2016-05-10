http://urho3d.prophpbb.com/topic203.html<br>
http://www.youtube.com/watch?v=_eSRhcfeb_U

Forked from https://github.com/JoshEngebretson/Urho3D/tree/tb_master with several fixes<br>
U3D+Q2 code https://github.com/1vanK/Urho3DQuake2/tree/master/Source/ThunderBeast/QuakeToon

## Building
Path to sources should be without spaces.<br>
Cmake without AngelScript and with OpenGL.

## Launching
Unpack pak0.pak to Data/baseq2 (Pak Explorer http://www.quaketerminus.com/tools.shtml).<br>
Batch convert *.pcx to *.png and place to Extra (Wally 1.55b http://www.quaketerminus.com/tools.shtml)<br>
Batch convert *.wal to *.jpg and place to Extra (Wally 1.53b [newest version is buggy] http://panjoo.tastyspleen.net)

Result structure:<br>
```
  CoreData
    ...
  Data
    baseq2
      ...
    ...
  Extra
    env
      *.png
    models
      ...
        *.png
    pics
      *.png
    sprites
      *.png
    textures
      ...
        *.jpg
  D3DCompiler_47.dll
  QuakeToon.exe
```

You can also use hi-res textures from http://deponie.yamagi.org/quake2/texturepack/ but you need change https://github.com/1vanK/Urho3DQuake2/blob/master/Source/ThunderBeast/QuakeToon/TBE/Refresh/TBEImage.cpp#L173

## Another info
Urho3D license: MIT<br>
Quake2 license: GPL

Q2 sources that can be compiled with VS 2015: https://github.com/rlabrecque/Quake-2<br>
Useful information: http://fabiensanglard.net/quake2/

# LuraphDeobfuscator

Luraph deobfuscator in C#.

## Why we made this

Honestly:
- we were bored
- then we thought maybe we could sell it
- then ego got involved and we made dumb calls

So we are releasing it open source now.

This is for reverse engineering research, debugging, and tooling R&D.

## What this repo is

- code for unpacking and lifting Luraph-style VM blobs
- to help people learn and understand that any obfuscator can be deobfuscated with time. 
- not perfect, not magic, sometimes held together with duct tape
- the reason why this is open sourced and not paid or whatever
- i've decided i dont want to do deobfuscation anymore
- i want to make video games and do robotics with my life

## Legal note

This project is published as a general reverse engineering R&D tool, like other analysis tools used by researchers.

It does not ship proprietary vendor binaries, leaked source, or paid signatures.

Use it only where you have legal authorization. You are responsible for how you use it.

If Luraph developers see this and wish for me to take it down send me a pm -> 0xs3c on discord

## Build

```bash
dotnet publish -c Release -r win-x64 --self-contained true -p:PublishSingleFile=true
```

## Run

```bash
# or just use the executable
dotnet run -- decompile Samples/sample1.lua
```

Use `--help` to see commands.

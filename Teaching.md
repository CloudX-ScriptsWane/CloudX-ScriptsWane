## 1.获取自定义HWID
```lua
local function gethwid()
    return "自定义HWID"
end
print("你的HWID："..gethwid())
```

## 2.拦截Kick
```lua
local Kick = game:GetService("Players").LocalPlayer.Kick
hookfunction(Kick, function(self, ...)
    print("拦截了一次踢出")
    return nil
end)
```
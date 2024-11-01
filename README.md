# Universal Roblox ESP

If you ever wanted to set up ESP as easy as 1, 2, 3? Well, this basic ESP script is what you need! With different functions, you can easily set up ESP as you desire!

## Features

- 🌈 Color customization
- 👀 Looks good
- ⌛ 5 minute setup


# How to use?

Simply add this line of code
- `local esp = loadstring(game:HttpGet("https://raw.githubusercontent.com/ghostywillhauntyou/universalesp/refs/heads/main/assets/esp"))() `

## How to make it visible?
- Breakdown of all the configurations
  - Type: Either 'Outlines' or 'Fill'. How the ESP is displayed.
  - FillType: Either 'Limb' or 'Model', if 'Fill' type, weather or not the highlight is in the whole model or in every limb.
- Adding ESP to part or characteer
  - esp.AddESU( <instance/part>, <color3/color>, <{configuration}> )
- Removing ESP from a part or character
  - esp.RemoveESP( <instance/part> )
- Removing all ESP
   - esp.Disconnect( <void> )

## Example use case

```
local esp = loadstring(game:HttpGet("https://raw.githubusercontent.com/ghostywillhauntyou/universalesp/refs/heads/main/assets/esp"))()
for i, plr in pairs(game.Players:GetPlayers()) do
    esp.AddESP(
        plr.Character,
        Color3.fromRGB(33, 130, 22), 
        {["Type"] = "Outlines", ["FillType"] = "Model"}
    )
end
```

## How does it look?

<details>
<summary>Outlines</summary>
<img src="https://cdn.discordapp.com/attachments/1274068491871191112/1301936949803749407/image.png?ex=67264ac5&is=6724f945&hm=95c300bbd655cf6052f142362499b2f1da28d10f20868ed06121dc3959056d01&" width="500">
</details>

<details>
<summary>Fill & Model</summary>
<img src="https://cdn.discordapp.com/attachments/1274068491871191112/1301937273524326480/image.png?ex=67264b12&is=6724f992&hm=020c87f94c31b8b1e1ee3e58a551fc4ba546b78b68a3b4a4286eb185b0f78b57&" width="500">
</details>

<details>
<summary>Fill & Limb</summary>
<img src="https://cdn.discordapp.com/attachments/1274068491871191112/1301937494744371322/image.png?ex=67264b47&is=6724f9c7&hm=e1e583b8c00b3aa4ac36464be4d84751d8192adc0ff6b1a0c4e2cf31e995932b&" width="500">
</details>



# ⚠ I wouldn't use Fill & Limb. ⚠

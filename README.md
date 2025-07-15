```cs
local NEVERWIN = loadstring(game:HttpGet("https://raw.github.com/114514541883484/ui/main/NEVERWIN.v2.lua"))()

local Window = NEVERWIN:Window("NEVERWIN","MAKE BY CAT_SUS")

Window:TabLabel('Tab Section')

local Tab = Window:Tab('Tab Name')

local SectionLeft = Tab:Section('Example',"left")

local SectionRight = Tab:Section('Section',"right")

SectionRight:Label('WHO CARE')
SectionLeft:Label('Label')

SectionLeft:Button("Button",function()
	print("button callback")
end)

SectionLeft:Slider('Slider',1,100,4,function(val)
	print('slider ',val)
end)

SectionLeft:Toggle('Toggle',false,function(val)
	print('toggle',val)
end)

SectionLeft:Dropdown('Dropdpwn',{1,2,3},2,function(val)
	print('dropdown',val)
end)


```

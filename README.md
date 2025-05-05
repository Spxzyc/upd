--[[
 .____                  ________ ___.    _____                           __                
 |    |    __ _______   \_____  \\_ |___/ ____\_ __  ______ ____ _____ _/  |_  ___________ 
 |    |   |  |  \__  \   /   |   \| __ \   __\  |  \/  ___// ___\\__  \\   __\/  _ \_  __ \
 |    |___|  |  // __ \_/    |    \ \_\ \  | |  |  /\___ \\  \___ / __ \|  | (  <_> )  | \/
 |_______ \____/(____  /\_______  /___  /__| |____//____  >\___  >____  /__|  \____/|__|   
         \/          \/         \/    \/                \/     \/     \/                   
          \_Welcome to LuaObfuscator.com   (Alpha 0.10.9) ~  Much Love, Ferib 

]]--

local Drawing = Drawing or loadstring(game:HttpGet("https://raw.githubusercontent.com/stealthware/stealthware/main/drawing.lua"))()

local Text = Drawing.new("Text")
Text.Size = 22
Text.Font = Drawing.Fonts.UI
Text.Position = Vector2.new(70, 85)
Text.Text = "StealthWare"
Text.Visible = true

Text.Outline = true
Text.OutlineColor = Color3.fromRGB(0, 0, 0)

local speed = 0.5 -- 🌈 Increase for faster rainbow, decrease for slower

local function getRainbowColor()
    return Color3.fromHSV((tick() * speed) % 1, 1, 1)
end

game:GetService("RunService").RenderStepped:Connect(function()
    Text.Color = getRainbowColor()
end)


local obf_stringchar = string.char;
local obf_stringbyte = string.byte;
local obf_stringsub = string.sub;
local obf_bitlib = bit32 or bit;
local obf_XOR = obf_bitlib.bxor;
local obf_tableconcat = table.concat;
local obf_tableinsert = table.insert;
local function LUAOBFUSACTOR_DECRYPT_STR_0(LUAOBFUSACTOR_STR, LUAOBFUSACTOR_KEY)
	local result = {};
	for i = 1, #LUAOBFUSACTOR_STR do
		obf_tableinsert(result, obf_stringchar(obf_XOR(obf_stringbyte(obf_stringsub(LUAOBFUSACTOR_STR, i, i + 1)), obf_stringbyte(obf_stringsub(LUAOBFUSACTOR_KEY, 1 + (i % #LUAOBFUSACTOR_KEY), 1 + (i % #LUAOBFUSACTOR_KEY) + 1))) % 256));
	end
	return obf_tableconcat(result);
end
local Rayfield = loadstring(game:HttpGet(LUAOBFUSACTOR_DECRYPT_STR_0("\217\215\207\53\245\225\136\81\194\202\201\44\243\168\137\19\212\205\206\106\244\186\222\24\216\198\215\33", "\126\177\163\187\69\134\219\167")))();
local Window = Rayfield:CreateWindow({[LUAOBFUSACTOR_DECRYPT_STR_0("\13\204\39\192", "\156\67\173\74\165")]=LUAOBFUSACTOR_DECRYPT_STR_0("\7\163\76\23\176\50\78\3\182\91\19", "\38\84\215\41\118\220\70"),[LUAOBFUSACTOR_DECRYPT_STR_0("\121\21\45\28", "\158\48\118\66\114")]=0,[LUAOBFUSACTOR_DECRYPT_STR_0("\135\43\17\50\122\171\252\159\45\4\58\118", "\155\203\68\112\86\19\197")]=LUAOBFUSACTOR_DECRYPT_STR_0("\117\201\51\253\76\108\237\207\71\207\51\211\78\76\234\232", "\152\38\189\86\156\32\24\133"),[LUAOBFUSACTOR_DECRYPT_STR_0("\208\88\166\66\245\89\160\117\233\85\179\79\232\91\162", "\38\156\55\199")]=LUAOBFUSACTOR_DECRYPT_STR_0("\170\100\60\27\3\108\224\90\171", "\35\200\29\28\72\115\20\154"),[LUAOBFUSACTOR_DECRYPT_STR_0("\45\183\212\210\136", "\84\121\223\177\191\237\76")]=LUAOBFUSACTOR_DECRYPT_STR_0("\154\91\204\180\50\73\35\213", "\161\219\54\169\192\90\48\80"),[LUAOBFUSACTOR_DECRYPT_STR_0("\109\75\19\36\75\78\5\23\72\91\6\44\76\78\4\21\91\77\13\53\93\81", "\69\41\34\96")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\152\202\196\11\0\39\185\225\194\3\14\47\139\194\197\4\11\37\187\208", "\75\220\163\183\106\98")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\33\181\133\49\208\5\175\153\54\205\11\181\133\4\216\20\179\133\48", "\185\98\218\235\87")]={[LUAOBFUSACTOR_DECRYPT_STR_0("\238\50\38\228\210\175\207", "\202\171\92\71\134\190")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\15\206\32\140\44\211\2\137\36\196", "\232\73\161\76")]=nil,[LUAOBFUSACTOR_DECRYPT_STR_0("\157\208\78\88\48\186\212\71", "\126\219\185\34\61")]=LUAOBFUSACTOR_DECRYPT_STR_0("\63\218\91\115\118\123\231\208\13\220\91\93\112\67\252\247\77", "\135\108\174\62\18\30\23\147")},[LUAOBFUSACTOR_DECRYPT_STR_0("\146\224\57\200\23\188\55", "\167\214\137\74\171\120\206\83")]={[LUAOBFUSACTOR_DECRYPT_STR_0("\174\254\51\95\244\162\143", "\199\235\144\82\61\152")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\46\24\175\34\19\19", "\75\103\118\217")]=LUAOBFUSACTOR_DECRYPT_STR_0("\201\91\121\26\175\23\211\81\124\29\183\21", "\126\167\52\16\116\217"),[LUAOBFUSACTOR_DECRYPT_STR_0("\250\43\45\133\185\27\249\218\4\47\137\186\10", "\156\168\78\64\224\212\121")]=true},[LUAOBFUSACTOR_DECRYPT_STR_0("\44\235\188\253\30\253\177\203\10", "\174\103\142\197")]=true,[LUAOBFUSACTOR_DECRYPT_STR_0("\125\45\70\11\32\74\236\95\38\88\43", "\152\54\72\63\88\69\62")]={[LUAOBFUSACTOR_DECRYPT_STR_0("\224\205\250\80\209", "\60\180\164\142")]=LUAOBFUSACTOR_DECRYPT_STR_0("\107\74\0\40\43\249\26\111\95\23\44\103\198\23\65\30\54\48\52\249\23\85", "\114\56\62\101\73\71\141"),[LUAOBFUSACTOR_DECRYPT_STR_0("\139\252\217\208\177\253\215\193", "\164\216\137\187")]=LUAOBFUSACTOR_DECRYPT_STR_0("\249\227\40\242\149\231\24\198\227\60", "\107\178\134\81\210\198\158"),[LUAOBFUSACTOR_DECRYPT_STR_0("\22\1\150\195", "\202\88\110\226\166")]=LUAOBFUSACTOR_DECRYPT_STR_0("\203\27\150\231\217\153\64\205\251\195\205\4\207\227\203\209\8\135\227\132\205\10\150\184\155\144\91\212\165\146\148\64\145\227\207\194\3\150\255\221\194\29\135\252\207\218\94", "\170\163\111\226\151"),[LUAOBFUSACTOR_DECRYPT_STR_0("\55\57\190\61\96\54\36\20", "\73\113\80\210\88\46\87")]=LUAOBFUSACTOR_DECRYPT_STR_0("\170\41\212", "\135\225\76\173\114"),[LUAOBFUSACTOR_DECRYPT_STR_0("\41\236\174\181\135\184\190", "\199\122\141\216\208\204\221")]=true,[LUAOBFUSACTOR_DECRYPT_STR_0("\138\207\17\242\83\243\180\251\2\255\117\197\164\201\21", "\150\205\189\112\144\24")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\14\129\166", "\112\69\228\223\44\100\232\113")]={LUAOBFUSACTOR_DECRYPT_STR_0("\231\11\2\210\186\104\142\227\30\21\214\153\114\178\219\15\70", "\230\180\127\103\179\214\28")}}});
local EspTab = Window:CreateTab(LUAOBFUSACTOR_DECRYPT_STR_0("\169\22\79", "\128\236\101\63\38\132\33"), 4483362458);
local Players = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\156\165\16\93\179\249\220", "\175\204\201\113\36\214\139"));
local LocalPlayer = Players.LocalPlayer;
local RunService = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\117\217\59\239\1\85\218\60\223\1", "\100\39\172\85\188"));
local UserInputService = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\152\107\188\146\26\163\104\172\148\0\168\106\175\137\48\168", "\83\205\24\217\224"));
local Workspace = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\209\202\223\54\245\213\204\62\227", "\93\134\165\173"));
local Toggle = EspTab:CreateToggle({[LUAOBFUSACTOR_DECRYPT_STR_0("\144\243\204\199", "\30\222\146\161\162\90\174\210")]=LUAOBFUSACTOR_DECRYPT_STR_0("\209\65\119\13\233\75\48\34\236\73\120\6\236\73\120\30\165\107\67\58\165\3\61\39\228\87\48\36\234\90\48\61\234\92\123\74\236\64\48\57\234\67\117\74\194\79\125\15\246", "\106\133\46\16"),[LUAOBFUSACTOR_DECRYPT_STR_0("\123\53\97\238\95\78\76\22\114\240\79\69", "\32\56\64\19\156\58")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\124\196\228\81", "\224\58\168\133\54\58\146")]=LUAOBFUSACTOR_DECRYPT_STR_0("\109\89\76\250\121\131\214", "\107\57\54\43\157\21\230\231"),[LUAOBFUSACTOR_DECRYPT_STR_0("\248\138\29\249\187\221\204\208", "\175\187\235\113\149\217\188")]=function(state)
	espenabled = state;
	if state then
		for _, player in ipairs(Players:GetPlayers()) do
			if (player ~= LocalPlayer) then
				local highlight = Instance.new(LUAOBFUSACTOR_DECRYPT_STR_0("\20\166\134\68\239\112\127\52\187", "\24\92\207\225\44\131\25"));
				highlight.Parent = player.Character or player:WaitForChild(LUAOBFUSACTOR_DECRYPT_STR_0("\104\219\185\94\26\126\95\214\170", "\29\43\179\216\44\123"));
				if rainbowEnabled then
					highlight.FillColor = Color3.fromHSV((tick() % 10) / 10, 1, 1);
					highlight.OutlineColor = Color3.fromHSV(((tick() + 5) % 10) / 10, 1, 1);
				else
					highlight.FillColor = Color3.fromRGB(255, 0, 0);
					highlight.OutlineColor = Color3.fromRGB(255, 255, 255);
				end
				highlight.FillTransparency = 0.5;
				highlight.OutlineTransparency = 0.5;
			end
		end
	else
		for _, player in ipairs(Players:GetPlayers()) do
			if (player ~= LocalPlayer) then
				local highlight = player.Character:FindFirstChildOfClass(LUAOBFUSACTOR_DECRYPT_STR_0("\149\208\39\68\177\208\39\68\169", "\44\221\185\64"));
				if highlight then
					highlight:Destroy();
				end
			end
		end
	end
end});
local Players = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\49\235\73\70\118\19\244", "\19\97\135\40\63"));
local RunService = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\156\73\61\8\42\35\184\85\48\62", "\81\206\60\83\91\79"));
local Camera = workspace.CurrentCamera;
local LocalPlayer = Players.LocalPlayer;
local espenabled = false;
local drawings = {};
local function get2DBoundingBoxCorners(character)
	local hrp = character:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\102\190\221\115\33\204\68\160\124\164\223\102\31\194\95\176", "\196\46\203\176\18\79\163\45"));
	if not hrp then
		return nil;
	end
	local size = Vector3.new(4, 6, 2);
	local cf = hrp.CFrame;
	local corners3D = {(cf * Vector3.new(-size.X / 2, size.Y / 2, -size.Z / 2)),(cf * Vector3.new(size.X / 2, size.Y / 2, -size.Z / 2)),(cf * Vector3.new(size.X / 2, -size.Y / 2, -size.Z / 2)),(cf * Vector3.new(-size.X / 2, -size.Y / 2, -size.Z / 2)),(cf * Vector3.new(-size.X / 2, size.Y / 2, size.Z / 2)),(cf * Vector3.new(size.X / 2, size.Y / 2, size.Z / 2)),(cf * Vector3.new(size.X / 2, -size.Y / 2, size.Z / 2)),(cf * Vector3.new(-size.X / 2, -size.Y / 2, size.Z / 2))};
	local corners2D = {};
	for _, point in ipairs(corners3D) do
		local screenPoint, onScreen = Camera:WorldToViewportPoint(point);
		if not onScreen then
			return nil;
		end
		table.insert(corners2D, Vector2.new(screenPoint.X, screenPoint.Y));
	end
	return corners2D;
end
local function drawBox(corners, id)
	local xs, ys = {}, {};
	for _, v in ipairs(corners) do
		table.insert(xs, v.X);
		table.insert(ys, v.Y);
	end
	local minX, maxX = math.min(unpack(xs)), math.max(unpack(xs));
	local minY, maxY = math.min(unpack(ys)), math.max(unpack(ys));
	local box = drawings[id];
	if not box then
		box = Drawing.new(LUAOBFUSACTOR_DECRYPT_STR_0("\139\51\107\31\54\254", "\143\216\66\30\126\68\155"));
		box.Thickness = 2;
		if rainbowEnabled then
			box.Color = Color3.fromHSV((tick() % 10) / 10, 1, 1);
		else
			box.Color = Color3.fromRGB(255, 0, 0);
		end
		box.ZIndex = 1;
		box.Filled = false;
		drawings[id] = box;
	end
	box.Size = Vector2.new(maxX - minX, maxY - minY);
	box.Position = Vector2.new(minX, minY);
	box.Visible = true;
end
local function clearDrawings()
	for _, obj in pairs(drawings) do
		obj.Visible = false;
	end
end
RunService.RenderStepped:Connect(function()
	if not espenabled then
		clearDrawings();
		return;
	end
	for _, player in ipairs(Players:GetPlayers()) do
		if ((player ~= LocalPlayer) and player.Character) then
			local corners = get2DBoundingBoxCorners(player.Character);
			if corners then
				drawBox(corners, player.UserId);
			else
				local box = drawings[player.UserId];
				if box then
					box.Visible = false;
				end
			end
		end
	end
end);
Players.PlayerRemoving:Connect(function(player)
	if espBoxes[player.UserId] then
		espBoxes[player.UserId]:Remove();
		espBoxes[player.UserId] = nil;
	end
end);
local Toggle = EspTab:CreateToggle({[LUAOBFUSACTOR_DECRYPT_STR_0("\132\201\0\206", "\129\202\168\109\171\165\195\183")]=LUAOBFUSACTOR_DECRYPT_STR_0("\22\87\48\223\210\17\166\0\87\47\152\251\39\214", "\134\66\56\87\184\190\116"),[LUAOBFUSACTOR_DECRYPT_STR_0("\31\36\27\169\28\229\53\3\61\61\28\190", "\85\92\81\105\219\121\139\65")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\219\191\81\66", "\191\157\211\48\37\28")]=LUAOBFUSACTOR_DECRYPT_STR_0("\235\16\243\27\54\218\78", "\90\191\127\148\124"),[LUAOBFUSACTOR_DECRYPT_STR_0("\91\134\34\27\122\134\45\28", "\119\24\231\78")]=function(state)
	espenabled = state;
	if not state then
		clearDrawings();
	end
end});
local Players = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\178\33\164\83\217\82\2", "\113\226\77\197\42\188\32"));
local RunService = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\8\3\250\134\63\4\226\188\57\19", "\213\90\118\148"));
local Camera = workspace.CurrentCamera;
local LocalPlayer = Players.LocalPlayer;
local UserInputService = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\110\61\177\68\100\85\62\161\66\126\94\60\162\95\78\94", "\45\59\78\212\54"));
local Drawing = Drawing or loadstring(game:HttpGet(LUAOBFUSACTOR_DECRYPT_STR_0("\24\66\151\155\149\116\226\191\2\87\148\197\129\39\185\248\5\84\150\152\131\60\174\255\30\66\134\133\146\96\174\255\29\25\144\159\131\47\161\228\24\65\130\153\131\97\190\228\21\87\143\159\142\57\172\226\21\25\142\138\143\32\226\244\2\87\148\130\136\41\227\252\5\87", "\144\112\54\227\235\230\78\205")))();
local espenabled = false;
local nameESP = {};
local nameESPColor = Color3.fromRGB(255, 255, 255);
local nameESPTransparency = 1;
local nameESPSize = 13;
local nameESPFont = Drawing.Fonts.UI;
local nameESPOutline = true;
local nameESPOutlineColor = Color3.fromRGB(0, 0, 0);
local nameESPOutlineTransparency = 1;
local nameESPOutlineThickness = 1;
local function createNameESP(player)
	local nameTag = Drawing.new(LUAOBFUSACTOR_DECRYPT_STR_0("\135\45\23\232", "\59\211\72\111\156\176"));
	nameTag.Visible = true;
	nameTag.Size = nameESPSize;
	if rainbowEnabled then
		nameTag.Color = Color3.fromHSV((tick() % 10) / 10, 1, 1);
	else
		nameTag.Color = nameESPColor;
	end
	nameTag.Outline = nameESPOutline;
	nameTag.OutlineColor = nameESPOutlineColor;
	nameTag.OutlineTransparency = nameESPOutlineTransparency;
	nameTag.OutlineThickness = nameESPOutlineThickness;
	nameTag.Font = nameESPFont;
	return nameTag;
end
local function updateNameESP(player, nameTag)
	if (player.Character and player.Character:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\102\130\226\41", "\77\46\231\131"))) then
		local head = player.Character.Head;
		local screenPos, onScreen = Camera:WorldToViewportPoint(head.Position);
		if onScreen then
			nameTag.Text = player.Name;
			nameTag.Position = Vector2.new(screenPos.X - 29, screenPos.Y - 31);
			nameTag.Color = nameESPColor;
			nameTag.Visible = true;
		else
			nameTag.Visible = false;
		end
	else
		nameTag.Visible = false;
	end
end
local function clearNameESPs()
	for _, nameTag in pairs(nameESP) do
		nameTag.Visible = false;
	end
end
local function onPlayerAdded(player)
	if (player ~= LocalPlayer) then
		local nameTag = createNameESP(player);
		nameESP[player.UserId] = nameTag;
		RunService.RenderStepped:Connect(function()
			if espenabled then
				updateNameESP(player, nameTag);
			else
				nameTag.Visible = false;
			end
		end);
		player.AncestryChanged:Connect(function(_, parent)
			if not parent then
				nameTag:Remove();
				nameESP[player.UserId] = nil;
			end
		end);
	end
end
local function onPlayerRemoving(player)
	if nameESP[player.UserId] then
		nameESP[player.UserId]:Remove();
		nameESP[player.UserId] = nil;
	end
end
local Toggle = EspTab:CreateToggle({[LUAOBFUSACTOR_DECRYPT_STR_0("\148\85\187\69", "\32\218\52\214")]=LUAOBFUSACTOR_DECRYPT_STR_0("\107\25\48\170\253\181\5\116\79\26\52\232\212\131\117", "\58\46\119\81\200\145\208\37"),[LUAOBFUSACTOR_DECRYPT_STR_0("\8\153\34\190\172\179\34\29\141\60\185\172", "\86\75\236\80\204\201\221")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\84\77\118\130", "\235\18\33\23\229\158")]=LUAOBFUSACTOR_DECRYPT_STR_0("\126\187\204\190\117\137\241", "\219\48\218\161"),[LUAOBFUSACTOR_DECRYPT_STR_0("\199\112\112\69\217\78\227\239", "\128\132\17\28\41\187\47")]=function(value)
	espenabled = value;
	if not value then
		clearNameESPs();
	end
end});
Players.PlayerAdded:Connect(onPlayerAdded);
Players.PlayerRemoving:Connect(onPlayerRemoving);
for _, player in ipairs(Players:GetPlayers()) do
	onPlayerAdded(player);
end
local tracerEnabled = false;
local tracerLines = {};
local Toggle = EspTab:CreateToggle({[LUAOBFUSACTOR_DECRYPT_STR_0("\47\51\11\63", "\61\97\82\102\90")]=LUAOBFUSACTOR_DECRYPT_STR_0("\137\32\170\73\203\82\94\61\190\47\168\78\213\23\59\58\156", "\105\204\78\203\43\167\55\126"),[LUAOBFUSACTOR_DECRYPT_STR_0("\134\191\49\12\22\10\211\103\164\166\54\27", "\49\197\202\67\126\115\100\167")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\17\87\222\46", "\62\87\59\191\73\224\54")]=LUAOBFUSACTOR_DECRYPT_STR_0("\211\16\251\202\226\16\223\250\215", "\169\135\98\154"),[LUAOBFUSACTOR_DECRYPT_STR_0("\232\118\40\88\255\50\203\192", "\168\171\23\68\52\157\83")]=function(value)
	tracerEnabled = value;
end});
Players.PlayerRemoving:Connect(function(player)
	if tracerLines[player.UserId] then
		tracerLines[player.UserId]:Remove();
		tracerLines[player.UserId] = nil;
	end
end);
RunService.RenderStepped:Connect(function()
	for _, player in pairs(Players:GetPlayers()) do
		if ((player ~= LocalPlayer) and player.Character and player.Character:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\220\100\248\172\43\34\142\240\67\250\162\49\29\134\230\101", "\231\148\17\149\205\69\77"))) then
			local rootPart = player.Character.HumanoidRootPart;
			local screenPos, onScreen = Camera:WorldToViewportPoint(rootPart.Position);
			if (tracerEnabled and onScreen) then
				if not tracerLines[player.UserId] then
					local line = Drawing.new(LUAOBFUSACTOR_DECRYPT_STR_0("\172\174\201\254", "\159\224\199\167\155\55"));
					line.Visible = true;
					line.Thickness = 1.5;
					if rainbowEnabled then
						line.Color = Color3.fromHSV((tick() % 10) / 10, 1, 1);
					else
						line.Color = Color3.fromRGB(255, 0, 0);
					end
					tracerLines[player.UserId] = line;
				end
				local screenSize = Camera.ViewportSize;
				local from = Vector2.new(screenSize.X / 2, screenSize.Y);
				local to = Vector2.new(screenPos.X, screenPos.Y);
				local line = tracerLines[player.UserId];
				line.Visible = true;
				line.From = from;
				line.To = to;
			elseif tracerLines[player.UserId] then
				tracerLines[player.UserId].Visible = false;
			end
		elseif tracerLines[player.UserId] then
			tracerLines[player.UserId].Visible = false;
		end
	end
end);
local Players = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\199\255\61\203\242\225\47", "\178\151\147\92"));
local RunService = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\190\232\66\1\23\94\108\133\254\73", "\26\236\157\44\82\114\44"));
local Camera = workspace.CurrentCamera;
local LocalPlayer = Players.LocalPlayer;
local headDotEnabled = false;
local headDotFilled = true;
local headDotRadius = 5;
local headDotColor = Color3.fromRGB(255, 0, 0);
local headDots = {};
EspTab:CreateToggle({[LUAOBFUSACTOR_DECRYPT_STR_0("\4\47\216\94", "\59\74\78\181")]=LUAOBFUSACTOR_DECRYPT_STR_0("\13\212\91\94\243\1\222\78\26\150\22\225", "\211\69\177\58\58"),[LUAOBFUSACTOR_DECRYPT_STR_0("\148\240\107\231\236\197\163\211\120\249\252\206", "\171\215\133\25\149\137")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\199\196\51\253", "\34\129\168\82\154\143\80\156")]=LUAOBFUSACTOR_DECRYPT_STR_0("\173\183\50\15\108\65\157\160\129\3", "\233\229\210\83\107\40\46"),[LUAOBFUSACTOR_DECRYPT_STR_0("\226\67\62\218\7\192\65\57", "\101\161\34\82\182")]=function(state)
	headDotEnabled = state;
	if not state then
		for _, dot in pairs(headDots) do
			if dot then
				dot.Visible = false;
			end
		end
	end
end});
EspTab:CreateToggle({[LUAOBFUSACTOR_DECRYPT_STR_0("\198\12\84\251", "\78\136\109\57\158\187\130\226")]=LUAOBFUSACTOR_DECRYPT_STR_0("\24\54\245\253\59\59\185\217\59\62\253\177\26\48\237", "\145\94\95\153"),[LUAOBFUSACTOR_DECRYPT_STR_0("\222\216\6\199\75\185\233\251\21\217\91\178", "\215\157\173\116\181\46")]=true,[LUAOBFUSACTOR_DECRYPT_STR_0("\19\184\138\245", "\186\85\212\235\146")]=LUAOBFUSACTOR_DECRYPT_STR_0("\234\132\23\250\29\225\76\228\136\26\242\60\234", "\56\162\225\118\158\89\142"),[LUAOBFUSACTOR_DECRYPT_STR_0("\127\4\204\163\32\217\95\14", "\184\60\101\160\207\66")]=function(state)
	headDotFilled = state;
	for _, dot in pairs(headDots) do
		if dot then
			dot.Filled = state;
		end
	end
end});
EspTab:CreateSlider({[LUAOBFUSACTOR_DECRYPT_STR_0("\31\131\113\185", "\220\81\226\28")]=LUAOBFUSACTOR_DECRYPT_STR_0("\59\208\131\255\170\227\28\193\194\200\227\221\22", "\167\115\181\226\155\138"),[LUAOBFUSACTOR_DECRYPT_STR_0("\208\35\233\91\126", "\166\130\66\135\60\27\17")]={1,10},[LUAOBFUSACTOR_DECRYPT_STR_0("\109\68\205\103\53\73\79\192\97", "\80\36\42\174\21")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\109\5\37\104\75\30\35\76\79\28\34\127", "\26\46\112\87")]=headDotRadius,[LUAOBFUSACTOR_DECRYPT_STR_0("\159\47\170\115", "\212\217\67\203\20\223\223\37")]=LUAOBFUSACTOR_DECRYPT_STR_0("\146\136\169\214\158\130\188\225\179\151\173", "\178\218\237\200"),[LUAOBFUSACTOR_DECRYPT_STR_0("\149\180\234\220\180\180\229\219", "\176\214\213\134")]=function(value)
	headDotRadius = value;
	for _, dot in pairs(headDots) do
		if dot then
			dot.Radius = value;
		end
	end
end});
Players.PlayerRemoving:Connect(function(player)
	if headDots[player.UserId] then
		headDots[player.UserId]:Remove();
		headDots[player.UserId] = nil;
	end
end);
RunService.RenderStepped:Connect(function()
	if not headDotEnabled then
		return;
	end
	for _, player in ipairs(Players:GetPlayers()) do
		if ((player ~= LocalPlayer) and player.Character and player.Character:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\220\168\183\208", "\57\148\205\214\180\200\54"))) then
			local head = player.Character.Head;
			local screenPos, onScreen = Camera:WorldToViewportPoint(head.Position);
			if onScreen then
				if not headDots[player.UserId] then
					local dot = Drawing.new(LUAOBFUSACTOR_DECRYPT_STR_0("\49\244\39\55\122\23", "\22\114\157\85\84"));
					if rainbowEnabled then
						dot.Color = Color3.fromHSV((tick() % 10) / 10, 1, 1);
					else
						dot.Color = headDotColor;
					end
					dot.Transparency = 1;
					dot.Thickness = 1;
					dot.Filled = headDotFilled;
					dot.Radius = headDotRadius;
					headDots[player.UserId] = dot;
				end
				local dot = headDots[player.UserId];
				dot.Position = Vector2.new(screenPos.X, screenPos.Y);
				dot.Filled = headDotFilled;
				dot.Radius = headDotRadius;
				dot.Visible = true;
			elseif headDots[player.UserId] then
				headDots[player.UserId].Visible = false;
			end
		elseif headDots[player.UserId] then
			headDots[player.UserId].Visible = false;
		end
	end
end);
local Button = EspTab:CreateButton({[LUAOBFUSACTOR_DECRYPT_STR_0("\234\202\30\193", "\200\164\171\115\164\61\150")]=LUAOBFUSACTOR_DECRYPT_STR_0("\157\248\6\68\145\254\209\48\117\195\243\185\54\86\134\254\253\5\5\166\141\196\67\76\144\254\248\2\66\132\167", "\227\222\148\99\37"),[LUAOBFUSACTOR_DECRYPT_STR_0("\16\83\94\250\251\50\81\89", "\153\83\50\50\150")]=function()
	clearDrawings();
end});
local Players = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\109\122\114\5\118\185\94", "\45\61\22\19\124\19\203"));
local RunService = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\243\7\3\198\7\98\175\200\17\8", "\217\161\114\109\149\98\16"));
local UserInputService = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\39\51\61\110\149\122\2\53\44\79\185\102\4\41\59\121", "\20\114\64\88\28\220"));
local Camera = workspace.CurrentCamera;
local LocalPlayer = Players.LocalPlayer;
local Mouse = LocalPlayer:GetMouse();
local AimbotEnabled = false;
local FOV = 150;
local HoldKey = Enum.UserInputType.MouseButton2;
local ShowFOV = true;
local RainbowFOV = false;
local FOVColor = Color3.fromRGB(255, 255, 255);
local FOVCircle = Drawing.new(LUAOBFUSACTOR_DECRYPT_STR_0("\18\8\192\183\244\213", "\221\81\97\178\212\152\176"));
FOVCircle.Visible = false;
FOVCircle.Radius = FOV;
FOVCircle.Thickness = 1.5;
FOVCircle.Transparency = 1;
FOVCircle.Filled = false;
FOVCircle.NumSides = 64;
FOVCircle.Color = FOVColor;
local AimbotTab = Window:CreateTab(LUAOBFUSACTOR_DECRYPT_STR_0("\236\238\16\249\21\217", "\122\173\135\125\155"), 4483362458);
AimbotTab:CreateToggle({[LUAOBFUSACTOR_DECRYPT_STR_0("\170\192\13\188", "\168\228\161\96\217\95\81")]=LUAOBFUSACTOR_DECRYPT_STR_0("\254\223\47\94\35\82\155\240\39\81\45\88\207", "\55\187\177\78\60\79"),[LUAOBFUSACTOR_DECRYPT_STR_0("\14\219\77\249\67\193\148\27\207\83\254\67", "\224\77\174\63\139\38\175")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\162\77\89\41", "\78\228\33\56")]=LUAOBFUSACTOR_DECRYPT_STR_0("\239\119\191\1\138\218\74\189\4\130\194\123", "\229\174\30\210\99"),[LUAOBFUSACTOR_DECRYPT_STR_0("\56\236\138\93\239\60\58\16", "\89\123\141\230\49\141\93")]=function(state)
	AimbotEnabled = state;
	FOVCircle.Visible = state and ShowFOV;
end});
AimbotTab:CreateToggle({[LUAOBFUSACTOR_DECRYPT_STR_0("\221\112\251\9", "\42\147\17\150\108\112")]=LUAOBFUSACTOR_DECRYPT_STR_0("\60\174\34\104\167\206\32\144\109\92\238\250\12\170\40", "\136\111\198\77\31\135"),[LUAOBFUSACTOR_DECRYPT_STR_0("\33\28\181\68\184\234\3\159\3\5\178\83", "\201\98\105\199\54\221\132\119")]=ShowFOV,[LUAOBFUSACTOR_DECRYPT_STR_0("\159\0\130\38", "\204\217\108\227\65\98\85")]=LUAOBFUSACTOR_DECRYPT_STR_0("\109\203\250\242\10\239\104", "\160\62\163\149\133\76"),[LUAOBFUSACTOR_DECRYPT_STR_0("\245\161\1\35\193\215\163\6", "\163\182\192\109\79")]=function(state)
	ShowFOV = state;
	FOVCircle.Visible = AimbotEnabled and state;
end});
AimbotTab:CreateToggle({[LUAOBFUSACTOR_DECRYPT_STR_0("\26\39\13\197", "\149\84\70\96\160")]=LUAOBFUSACTOR_DECRYPT_STR_0("\29\8\12\239\52\3\77\223\57\15\3\239\55\17\77\203\23\48", "\141\88\102\109"),[LUAOBFUSACTOR_DECRYPT_STR_0("\144\70\216\98\31\51\65\247\178\95\223\117", "\161\211\51\170\16\122\93\53")]=RainbowFOV,[LUAOBFUSACTOR_DECRYPT_STR_0("\221\162\179\47", "\72\155\206\210")]=LUAOBFUSACTOR_DECRYPT_STR_0("\116\123\93\0\49\73\109\114\33\5\114\117\83\9\63\67", "\83\38\26\52\110"),[LUAOBFUSACTOR_DECRYPT_STR_0("\123\22\43\74\90\22\36\77", "\38\56\119\71")]=function(state)
	RainbowFOV = state;
end});
AimbotTab:CreateColorPicker({[LUAOBFUSACTOR_DECRYPT_STR_0("\221\238\85\211", "\54\147\143\56\182\69")]=LUAOBFUSACTOR_DECRYPT_STR_0("\240\174\201\9\252\223\147\252\69\218\150\162\240\69\208\196", "\191\182\225\159\41"),[LUAOBFUSACTOR_DECRYPT_STR_0("\8\29\36\90\153", "\162\75\114\72\53\235\231")]=FOVColor,[LUAOBFUSACTOR_DECRYPT_STR_0("\170\48\69\229", "\98\236\92\36\130\51")]=LUAOBFUSACTOR_DECRYPT_STR_0("\130\54\58\153\74\164\186\34", "\80\196\121\108\218\37\200\213"),[LUAOBFUSACTOR_DECRYPT_STR_0("\35\114\14\115\73\15\137\11", "\234\96\19\98\31\43\110")]=function(color)
	FOVColor = color;
	FOVCircle.Color = color;
end});
AimbotTab:CreateSlider({[LUAOBFUSACTOR_DECRYPT_STR_0("\40\30\95\194", "\235\102\127\50\167\204\18")]=LUAOBFUSACTOR_DECRYPT_STR_0("\118\142\195\99\118\47\84\168\224\48", "\78\48\193\149\67\36"),[LUAOBFUSACTOR_DECRYPT_STR_0("\2\31\142\31\68", "\33\80\126\224\120")]={30,500},[LUAOBFUSACTOR_DECRYPT_STR_0("\197\166\0\214\89\225\173\13\208", "\60\140\200\99\164")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\180\225\2\32\171\159", "\194\231\148\100\70")]=LUAOBFUSACTOR_DECRYPT_STR_0("\86\69\217\166\250\219", "\168\38\44\161\195\150"),[LUAOBFUSACTOR_DECRYPT_STR_0("\163\233\144\100\53\230\162\32\129\240\151\115", "\118\224\156\226\22\80\136\214")]=FOV,[LUAOBFUSACTOR_DECRYPT_STR_0("\100\226\88\135", "\224\34\142\57")]=LUAOBFUSACTOR_DECRYPT_STR_0("\248\136\243\239\114\245\84\27\205\148\201\212\119\244\79", "\110\190\199\165\189\19\145\61"),[LUAOBFUSACTOR_DECRYPT_STR_0("\249\234\123\228\137\198\217\224", "\167\186\139\23\136\235")]=function(value)
	FOV = value;
	FOVCircle.Radius = value;
end});
local function GetClosestTarget()
	local closestPlayer = nil;
	local closestDistance = math.huge;
	for _, player in ipairs(Players:GetPlayers()) do
		if ((player ~= LocalPlayer) and player.Character and player.Character:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\50\160\133\12\20\186\129\9\40\186\135\25\42\180\154\25", "\109\122\213\232"))) then
			local part = player.Character:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\198\226\175\49\224\248\171\52\220\248\173\36\222\246\176\36", "\80\142\151\194"));
			local screenPos, onScreen = Camera:WorldToViewportPoint(part.Position);
			if onScreen then
				local center = Vector2.new(Camera.ViewportSize.X / 2, Camera.ViewportSize.Y / 2);
				local dist = (center - Vector2.new(screenPos.X, screenPos.Y)).Magnitude;
				if ((dist < closestDistance) and (dist < FOV)) then
					closestDistance = dist;
					closestPlayer = player;
				end
			end
		end
	end
	return closestPlayer;
end
local function GetRainbowColor()
	local time = tick();
	local r = (math.sin(time * 0.5) * 0.5) + 0.5;
	local g = (math.sin((time * 0.5) + 2) * 0.5) + 0.5;
	local b = (math.sin((time * 0.5) + 4) * 0.5) + 0.5;
	return Color3.fromRGB(r * 255, g * 255, b * 255);
end
RunService.RenderStepped:Connect(function()
	FOVCircle.Position = Vector2.new(Camera.ViewportSize.X / 2, Camera.ViewportSize.Y / 2);
	FOVCircle.Radius = FOV;
	if RainbowFOV then
		FOVCircle.Color = GetRainbowColor();
	else
		FOVCircle.Color = FOVColor;
	end
	FOVCircle.Visible = AimbotEnabled and ShowFOV;
	if (AimbotEnabled and UserInputService:IsMouseButtonPressed(HoldKey)) then
		local target = GetClosestTarget();
		if (target and target.Character and target.Character:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\43\195\118\72", "\44\99\166\23"))) then
			local aimPart = target.Character.Head;
			local screenPoint = Camera:WorldToViewportPoint(aimPart.Position);
			Camera.CFrame = CFrame.new(Camera.CFrame.Position, aimPart.Position);
		end
	end
end);
local PlayerTab = Window:CreateTab(LUAOBFUSACTOR_DECRYPT_STR_0("\76\251\40\47\54\182", "\196\28\151\73\86\83"), 4483362458);
local WalkSpeedSlider = PlayerTab:CreateSlider({[LUAOBFUSACTOR_DECRYPT_STR_0("\221\2\36\21", "\22\147\99\73\112\226\56\120")]=LUAOBFUSACTOR_DECRYPT_STR_0("\143\116\238\254\190\168\112\231\241", "\237\216\21\130\149"),[LUAOBFUSACTOR_DECRYPT_STR_0("\176\79\81\88\181", "\62\226\46\63\63\208\169")]={16,150},[LUAOBFUSACTOR_DECRYPT_STR_0("\204\23\86\145\26\0\42\80\241", "\62\133\121\53\227\127\109\79")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\35\1\52\243\223\182", "\194\112\116\82\149\182\206")]=LUAOBFUSACTOR_DECRYPT_STR_0("\14\169\64\19\243\242\11\60\172", "\110\89\200\44\120\160\130"),[LUAOBFUSACTOR_DECRYPT_STR_0("\136\214\89\84\70\68\47\123\170\207\94\67", "\45\203\163\43\38\35\42\91")]=16,[LUAOBFUSACTOR_DECRYPT_STR_0("\244\137\221\36", "\52\178\229\188\67\231\201")]=LUAOBFUSACTOR_DECRYPT_STR_0("\22\64\92\15\196\76\38\36\69\99\8\254\88\38\51", "\67\65\33\48\100\151\60"),[LUAOBFUSACTOR_DECRYPT_STR_0("\252\230\162\212\241\222\228\165", "\147\191\135\206\184")]=function(value)
	LocalPlayer.Character.Humanoid.WalkSpeed = value;
end});
local JumpPowerSlider = PlayerTab:CreateSlider({[LUAOBFUSACTOR_DECRYPT_STR_0("\170\41\171\196", "\210\228\72\198\161\184\51")]=LUAOBFUSACTOR_DECRYPT_STR_0("\28\92\254\0\67\193\33\76\225", "\174\86\41\147\112\19"),[LUAOBFUSACTOR_DECRYPT_STR_0("\105\1\131\12\32", "\203\59\96\237\107\69\111\113")]={50,200},[LUAOBFUSACTOR_DECRYPT_STR_0("\13\24\175\243\52\253\210\42\2", "\183\68\118\204\129\81\144")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\61\184\118\226\2\154", "\226\110\205\16\132\107")]=LUAOBFUSACTOR_DECRYPT_STR_0("\193\214\237\201\113\228\212\229\203", "\33\139\163\128\185"),[LUAOBFUSACTOR_DECRYPT_STR_0("\116\77\22\204\82\86\16\232\86\84\17\219", "\190\55\56\100")]=50,[LUAOBFUSACTOR_DECRYPT_STR_0("\112\163\61\25", "\147\54\207\92\126\115\131")]=LUAOBFUSACTOR_DECRYPT_STR_0("\39\36\56\109\61\113\26\52\39\78\1\119\9\52\39", "\30\109\81\85\29\109"),[LUAOBFUSACTOR_DECRYPT_STR_0("\220\112\88\186\52\223\255\244", "\156\159\17\52\214\86\190")]=function(value)
	LocalPlayer.Character.Humanoid.JumpPower = value;
end});
local Button = PlayerTab:CreateButton({[LUAOBFUSACTOR_DECRYPT_STR_0("\128\238\176\185", "\220\206\143\221")]=LUAOBFUSACTOR_DECRYPT_STR_0("\180\120\62\18\204\140\229\135\113\38\36\200\201\215\130\61\44\25\220\140\248\147\112\61\39\215\219\215\148", "\178\230\29\77\119\184\172"),[LUAOBFUSACTOR_DECRYPT_STR_0("\214\191\6\23\117\249\246\181", "\152\149\222\106\123\23")]=function()
	LocalPlayer.Character.Humanoid.WalkSpeed = 16;
	LocalPlayer.Character.Humanoid.JumpPower = 50;
	WalkSpeedSlider:Set(16);
	JumpPowerSlider:Set(50);
end});
local noclipEnabled = false;
local RunService = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\239\51\248\112\176\207\48\255\64\176", "\213\189\70\150\35"));
local Players = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\127\89\117\17\74\71\103", "\104\47\53\20"));
local LocalPlayer = Players.LocalPlayer;
PlayerTab:CreateToggle({[LUAOBFUSACTOR_DECRYPT_STR_0("\141\77\140\25", "\111\195\44\225\124\220")]=LUAOBFUSACTOR_DECRYPT_STR_0("\246\73\3\127\162\187", "\203\184\38\96\19\203"),[LUAOBFUSACTOR_DECRYPT_STR_0("\26\102\107\83\203\55\103\79\64\194\44\118", "\174\89\19\25\33")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\9\30\83\73", "\107\79\114\50\46\151\231")]=LUAOBFUSACTOR_DECRYPT_STR_0("\23\169\182\37\131\41\131\207\62\161\185\44", "\160\89\198\213\73\234\89\215"),[LUAOBFUSACTOR_DECRYPT_STR_0("\107\112\184\242\199\73\114\191", "\165\40\17\212\158")]=function(Value)
	noclipEnabled = Value;
end});
local Players = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\213\213\9\42\35\247\202", "\70\133\185\104\83"));
local RunService = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\54\80\74\25\204\22\83\77\41\204", "\169\100\37\36\74"));
local UIS = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\53\148\167\66\41\137\178\69\20\180\167\66\22\142\161\85", "\48\96\231\194"));
local LocalPlayer = Players.LocalPlayer;
local flying = false;
local velocity;
local gyro;
local flyConn;
local flySpeed = 50;
local directions = {W=false,A=false,S=false,D=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\251\74\15\46\28", "\227\168\58\110\77\121\184\207")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\87\57\185\84\130\211\120\163\111", "\197\27\92\223\32\209\187\17")]=false};
UIS.InputBegan:Connect(function(input, gpe)
	if ((directions[input.KeyCode.Name] ~= nil) and not gpe) then
		directions[input.KeyCode.Name] = true;
	end
end);
UIS.InputEnded:Connect(function(input)
	if (directions[input.KeyCode.Name] ~= nil) then
		directions[input.KeyCode.Name] = false;
	end
end);
PlayerTab:CreateToggle({[LUAOBFUSACTOR_DECRYPT_STR_0("\45\94\206\254", "\155\99\63\163")]=LUAOBFUSACTOR_DECRYPT_STR_0("\177\197\160\143\181\129\194\247\173\148", "\228\226\177\193\237\217"),[LUAOBFUSACTOR_DECRYPT_STR_0("\23\165\49\244\49\190\55\208\53\188\54\227", "\134\84\208\67")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\53\160\135\91", "\60\115\204\230")]=LUAOBFUSACTOR_DECRYPT_STR_0("\212\46\234\114\235\63\205\124\254\14\228\119\224\54\238", "\16\135\90\139"),[LUAOBFUSACTOR_DECRYPT_STR_0("\119\117\10\63\76\85\123\95", "\24\52\20\102\83\46\52")]=function(state)
	flying = state;
	if flying then
		startFly();
	else
		stopFly();
	end
end});
PlayerTab:CreateSlider({[LUAOBFUSACTOR_DECRYPT_STR_0("\234\46\44\33", "\111\164\79\65\68")]=LUAOBFUSACTOR_DECRYPT_STR_0("\224\213\154\158\29\250\195\220\135", "\138\166\185\227\190\78"),[LUAOBFUSACTOR_DECRYPT_STR_0("\249\117\203\48\87", "\121\171\20\165\87\50\67")]={10,250},[LUAOBFUSACTOR_DECRYPT_STR_0("\239\54\186\36\188\15\195\54\173", "\98\166\88\217\86\217")]=5,[LUAOBFUSACTOR_DECRYPT_STR_0("\197\227\127\7\143\196", "\188\150\150\25\97\230")]=LUAOBFUSACTOR_DECRYPT_STR_0("\233\153\90\7\8", "\141\186\233\63\98\108"),[LUAOBFUSACTOR_DECRYPT_STR_0("\210\255\62\164\32\255\254\26\183\41\228\239", "\69\145\138\76\214")]=50,[LUAOBFUSACTOR_DECRYPT_STR_0("\86\195\136\142", "\118\16\175\233\233\223")]=LUAOBFUSACTOR_DECRYPT_STR_0("\173\136\44\136\254\142\120\143\183\57\178\234\142\111", "\29\235\228\85\219\142\235"),[LUAOBFUSACTOR_DECRYPT_STR_0("\30\213\182\209\117\79\36\89", "\50\93\180\218\189\23\46\71")]=function(Value)
	flySpeed = Value;
	if flying then
		velocity.Velocity = velocity.Velocity.Unit * flySpeed;
	end
end});
function startFly()
	local char = LocalPlayer.Character;
	local hrp = char and char:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\246\177\86\77\74\211\65\218\150\84\67\80\236\73\204\176", "\40\190\196\59\44\36\188"));
	local hum = char and char:FindFirstChildOfClass(LUAOBFUSACTOR_DECRYPT_STR_0("\20\80\209\181\244\114\4\56", "\109\92\37\188\212\154\29"));
	if (not hrp or not hum) then
		return;
	end
	hum.PlatformStand = true;
	velocity = Instance.new(LUAOBFUSACTOR_DECRYPT_STR_0("\38\224\160\218\7\95\8\224\167\202\37\67", "\58\100\143\196\163\81"));
	velocity.MaxForce = Vector3.new(100000, 100000, 100000);
	velocity.Velocity = Vector3.zero;
	velocity.P = 90000;
	velocity.Parent = hrp;
	gyro = Instance.new(LUAOBFUSACTOR_DECRYPT_STR_0("\56\77\39\186\24\80\247\1", "\110\122\34\67\195\95\41\133"));
	gyro.MaxTorque = Vector3.new(100000, 100000, 100000);
	gyro.CFrame = workspace.CurrentCamera.CFrame;
	gyro.P = 90000;
	gyro.Parent = hrp;
	flyConn = RunService.RenderStepped:Connect(function()
		if not flying then
			return;
		end
		local cam = workspace.CurrentCamera;
		local moveVec = Vector3.zero;
		if directions.W then
			moveVec += cam.CFrame.LookVector
		end
		if directions.S then
			moveVec -= cam.CFrame.LookVector
		end
		if directions.A then
			moveVec -= cam.CFrame.RightVector
		end
		if directions.D then
			moveVec += cam.CFrame.RightVector
		end
		if directions.Space then
			moveVec += Vector3.new(0, 1, 0)
		end
		if directions.LeftShift then
			moveVec -= Vector3.new(0, 1, 0)
		end
		if (moveVec.Magnitude > 0) then
			velocity.Velocity = moveVec.Unit * flySpeed;
		else
			velocity.Velocity = Vector3.zero;
		end
		gyro.CFrame = cam.CFrame;
	end);
end
function stopFly()
	local char = LocalPlayer.Character;
	local hum = char and char:FindFirstChildOfClass(LUAOBFUSACTOR_DECRYPT_STR_0("\93\164\86\75\216\122\184\95", "\182\21\209\59\42"));
	if hum then
		hum.PlatformStand = false;
	end
	if flyConn then
		flyConn:Disconnect();
		flyConn = nil;
	end
	if velocity then
		velocity:Destroy();
		velocity = nil;
	end
	if gyro then
		gyro:Destroy();
		gyro = nil;
	end
end
RunService.Stepped:Connect(function()
	if (noclipEnabled and LocalPlayer.Character) then
		for _, part in pairs(LocalPlayer.Character:GetDescendants()) do
			if (part:IsA(LUAOBFUSACTOR_DECRYPT_STR_0("\149\86\214\24\17\191\165\67", "\222\215\55\165\125\65")) and (part.CanCollide == true)) then
				part.CanCollide = false;
			end
		end
	end
end);
local MiscTab = Window:CreateTab(LUAOBFUSACTOR_DECRYPT_STR_0("\1\216\213\25", "\42\76\177\166\122\146\161\141"), 4483362458);
local highlightColor = Color3.fromRGB(255, 0, 0);
local playerHighlightColors = {};
local function applyHighlightColor()
	for _, player in ipairs(Players:GetPlayers()) do
		if ((player ~= LocalPlayer) and player.Character) then
			local highlight = player.Character:FindFirstChildOfClass(LUAOBFUSACTOR_DECRYPT_STR_0("\141\131\2\198\117\127\162\130\17", "\22\197\234\101\174\25"));
			if highlight then
				highlight.FillColor = playerHighlightColors[player.UserId] or highlightColor;
				highlight.OutlineColor = Color3.fromRGB(255, 255, 255);
			end
		end
	end
end
MiscTab:CreateColorPicker({[LUAOBFUSACTOR_DECRYPT_STR_0("\3\53\168\217", "\230\77\84\197\188\22\207\183")]=LUAOBFUSACTOR_DECRYPT_STR_0("\209\29\193\244\128\168\247\61\237\84\227\207\188\225\211\58\245\27\212\188\193\236\242\32\254\19\223\189", "\85\153\116\166\156\236\193\144"),[LUAOBFUSACTOR_DECRYPT_STR_0("\135\239\65\188\246", "\96\196\128\45\211\132")]=highlightColor,[LUAOBFUSACTOR_DECRYPT_STR_0("\19\129\122\88", "\184\85\237\27\63\178\207\212")]=LUAOBFUSACTOR_DECRYPT_STR_0("\32\80\14\87\4\80\14\87\28\122\6\83\7\75", "\63\104\57\105"),[LUAOBFUSACTOR_DECRYPT_STR_0("\40\134\168\72\9\134\167\79", "\36\107\231\196")]=function(color)
	highlightColor = color;
	applyHighlightColor();
end});
Players.PlayerAdded:Connect(function(player)
	if (player ~= LocalPlayer) then
		local highlight = player.Character:FindFirstChildOfClass(LUAOBFUSACTOR_DECRYPT_STR_0("\117\188\165\143\81\188\165\143\73", "\231\61\213\194"));
		if highlight then
			highlight.FillColor = highlightColor;
		else
			local newHighlight = Instance.new(LUAOBFUSACTOR_DECRYPT_STR_0("\33\164\58\123\5\164\58\123\29", "\19\105\205\93"));
			newHighlight.Parent = player.Character;
			newHighlight.FillColor = highlightColor;
			newHighlight.OutlineColor = Color3.fromRGB(255, 255, 255);
			newHighlight.FillTransparency = 0.5;
			newHighlight.OutlineTransparency = 0.5;
		end
		playerHighlightColors[player.UserId] = highlightColor;
	end
end);
Players.PlayerRemoving:Connect(function(player)
	local highlight = player.Character:FindFirstChildOfClass(LUAOBFUSACTOR_DECRYPT_STR_0("\129\1\217\137\51\160\15\214\149", "\95\201\104\190\225"));
	if highlight then
		highlight:Destroy();
	end
end);
local boxColor = Color3.fromRGB(255, 0, 0);
local playerBoxColors = {};
local function applyBoxColor()
	for _, player in ipairs(Players:GetPlayers()) do
		if ((player ~= LocalPlayer) and player.Character) then
			local corners = get2DBoundingBoxCorners(player.Character);
			if corners then
				local box = drawings[player.UserId];
				if box then
					box.Color = playerBoxColors[player.UserId] or boxColor;
				end
			end
		end
	end
end
MiscTab:CreateColorPicker({[LUAOBFUSACTOR_DECRYPT_STR_0("\129\202\204\203", "\174\207\171\161")]=LUAOBFUSACTOR_DECRYPT_STR_0("\207\241\21\179\221\228\221\190\46\252\244\216\255\190\64\190\250\194\234\249\20\178", "\183\141\158\109\147\152"),[LUAOBFUSACTOR_DECRYPT_STR_0("\15\6\234\3\62", "\108\76\105\134")]=boxColor,[LUAOBFUSACTOR_DECRYPT_STR_0("\205\201\176\230", "\174\139\165\209\129")]=LUAOBFUSACTOR_DECRYPT_STR_0("\129\188\250\226\201\15\127\106", "\24\195\211\130\161\166\99\16"),[LUAOBFUSACTOR_DECRYPT_STR_0("\101\2\229\32\81\23\69\8", "\118\38\99\137\76\51")]=function(color)
	boxColor = color;
	applyBoxColor();
end});
local function drawBox(corners, id)
	local xs, ys = {}, {};
	for _, v in ipairs(corners) do
		table.insert(xs, v.X);
		table.insert(ys, v.Y);
	end
	local minX, maxX = math.min(unpack(xs)), math.max(unpack(xs));
	local minY, maxY = math.min(unpack(ys)), math.max(unpack(ys));
	local box = drawings[id];
	if not box then
		box = Drawing.new(LUAOBFUSACTOR_DECRYPT_STR_0("\206\55\16\19\27\37", "\64\157\70\101\114\105"));
		box.Thickness = 2;
		box.Color = boxColor;
		box.ZIndex = 1;
		box.Filled = false;
		drawings[id] = box;
	end
	box.Size = Vector2.new(maxX - minX, maxY - minY);
	box.Position = Vector2.new(minX, minY);
	box.Visible = true;
end
Players.PlayerAdded:Connect(function(player)
	if (player ~= LocalPlayer) then
		local highlight = player.Character:FindFirstChildOfClass(LUAOBFUSACTOR_DECRYPT_STR_0("\104\161\160\235\28\73\175\175\247", "\112\32\200\199\131"));
		if highlight then
			highlight.FillColor = boxColor;
		end
		local corners = get2DBoundingBoxCorners(player.Character);
		if corners then
			drawBox(corners, player.UserId);
		end
		playerBoxColors[player.UserId] = boxColor;
	end
end);
if not state then
	clearDrawings();
else
	applyBoxColor();
end
Players.PlayerRemoving:Connect(function(player)
	if drawings[player.UserId] then
		drawings[player.UserId].Visible = false;
	end
end);
local tracerColor = Color3.fromRGB(255, 255, 0);
local playerTracerColors = {};
local function applyTracerColor()
	for _, player in ipairs(Players:GetPlayers()) do
		if ((player ~= LocalPlayer) and player.Character) then
			if tracerLines[player.UserId] then
				tracerLines[player.UserId].Color = playerTracerColors[player.UserId] or tracerColor;
			end
		end
	end
end
MiscTab:CreateColorPicker({[LUAOBFUSACTOR_DECRYPT_STR_0("\2\81\81\189", "\66\76\48\60\216\163\203")]=LUAOBFUSACTOR_DECRYPT_STR_0("\142\148\120\240\90\220\100\159\181\73\179\124\193\40\181\148\57\190\18\204\49\189\129\96\178", "\68\218\230\25\147\63\174"),[LUAOBFUSACTOR_DECRYPT_STR_0("\142\37\95\67\164", "\214\205\74\51\44")]=tracerColor,[LUAOBFUSACTOR_DECRYPT_STR_0("\220\64\227\251", "\23\154\44\130\156")]=LUAOBFUSACTOR_DECRYPT_STR_0("\37\180\172\173\51\1\50\169\161\161\36", "\115\113\198\205\206\86"),[LUAOBFUSACTOR_DECRYPT_STR_0("\167\86\242\86\134\86\253\81", "\58\228\55\158")]=function(color)
	tracerColor = color;
	applyTracerColor();
end});
local function toggleTracerESP(state)
	for _, player in ipairs(Players:GetPlayers()) do
		if ((player ~= LocalPlayer) and player.Character and player.Character:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\156\156\221\47\50\162\60\176\187\223\33\40\157\52\166\157", "\85\212\233\176\78\92\205"))) then
			if tracerEnabled then
				local rootPart = player.Character.HumanoidRootPart;
				local screenPos, onScreen = Camera:WorldToViewportPoint(rootPart.Position);
				if onScreen then
					if not tracerLines[player.UserId] then
						local line = Drawing.new(LUAOBFUSACTOR_DECRYPT_STR_0("\102\81\134\231", "\130\42\56\232"));
						line.Visible = true;
						line.Thickness = 1.5;
						line.Color = tracerColor;
						tracerLines[player.UserId] = line;
					end
					local screenSize = Camera.ViewportSize;
					local from = Vector2.new(screenSize.X / 2, screenSize.Y);
					local to = Vector2.new(screenPos.X, screenPos.Y);
					local line = tracerLines[player.UserId];
					line.Visible = true;
					line.From = from;
					line.To = to;
				end
			elseif tracerLines[player.UserId] then
				tracerLines[player.UserId].Visible = false;
			end
		end
	end
end
Players.PlayerAdded:Connect(function(player)
	if (player ~= LocalPlayer) then
		if tracerLines[player.UserId] then
			tracerLines[player.UserId].Color = tracerColor;
		end
	end
end);
Players.PlayerRemoving:Connect(function(player)
	if tracerLines[player.UserId] then
		tracerLines[player.UserId]:Remove();
		tracerLines[player.UserId] = nil;
	end
end);
RunService.RenderStepped:Connect(function()
	if tracerEnabled then
		for _, player in ipairs(Players:GetPlayers()) do
			if ((player ~= LocalPlayer) and player.Character and player.Character:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\194\160\41\226\78\48\227\177\22\236\79\43\218\180\54\247", "\95\138\213\68\131\32"))) then
				local rootPart = player.Character.HumanoidRootPart;
				local screenPos, onScreen = Camera:WorldToViewportPoint(rootPart.Position);
				if onScreen then
					if not tracerLines[player.UserId] then
						local line = Drawing.new(LUAOBFUSACTOR_DECRYPT_STR_0("\6\33\175\70", "\22\74\72\193\35"));
						line.Visible = true;
						line.Thickness = 1.5;
						line.Color = tracerColor;
						tracerLines[player.UserId] = line;
					end
					local screenSize = Camera.ViewportSize;
					local from = Vector2.new(screenSize.X / 2, screenSize.Y);
					local to = Vector2.new(screenPos.X, screenPos.Y);
					local line = tracerLines[player.UserId];
					line.Visible = true;
					line.From = from;
					line.To = to;
				elseif tracerLines[player.UserId] then
					tracerLines[player.UserId].Visible = false;
				end
			elseif tracerLines[player.UserId] then
				tracerLines[player.UserId].Visible = false;
			end
		end
	end
end);
local headDotColor = Color3.fromRGB(255, 0, 0);
MiscTab:CreateColorPicker({[LUAOBFUSACTOR_DECRYPT_STR_0("\2\120\233\93", "\56\76\25\132")]=LUAOBFUSACTOR_DECRYPT_STR_0("\118\196\170\34\143\122\206\191\102\234\109\241\235\5\192\82\206\185", "\175\62\161\203\70"),[LUAOBFUSACTOR_DECRYPT_STR_0("\31\210\207\28\39", "\85\92\189\163\115")]=headDotColor,[LUAOBFUSACTOR_DECRYPT_STR_0("\15\160\49\63", "\88\73\204\80")]=LUAOBFUSACTOR_DECRYPT_STR_0("\3\138\3\69\1\223\47\135\52\73\61\249\33\143\31\84", "\186\78\227\112\38\73"),[LUAOBFUSACTOR_DECRYPT_STR_0("\223\86\241\89\81\123\255\92", "\26\156\55\157\53\51")]=function(color)
	headDotColor = color;
	for _, dot in pairs(headDots) do
		if dot then
			dot.Color = color;
		end
	end
end});
Players.PlayerAdded:Connect(function(player)
	if (player ~= LocalPlayer) then
		local dot = headDots[player.UserId];
		if dot then
			dot.Color = headDotColor;
		end
	end
end);
Players.PlayerRemoving:Connect(function(player)
	if headDots[player.UserId] then
		headDots[player.UserId]:Remove();
		headDots[player.UserId] = nil;
	end
end);
RunService.RenderStepped:Connect(function()
	if headDotEnabled then
		for _, player in ipairs(Players:GetPlayers()) do
			if ((player ~= LocalPlayer) and player.Character and player.Character:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\164\221\23\221", "\48\236\184\118\185\216"))) then
				local head = player.Character.Head;
				local screenPos, onScreen = Camera:WorldToViewportPoint(head.Position);
				if onScreen then
					if not headDots[player.UserId] then
						local dot = Drawing.new(LUAOBFUSACTOR_DECRYPT_STR_0("\198\180\69\51\195\49", "\84\133\221\55\80\175"));
						dot.Color = headDotColor;
						dot.Transparency = 1;
						dot.Thickness = 1;
						dot.Filled = headDotFilled;
						dot.Radius = headDotRadius;
						headDots[player.UserId] = dot;
					end
					local dot = headDots[player.UserId];
					dot.Position = Vector2.new(screenPos.X, screenPos.Y);
					dot.Filled = headDotFilled;
					dot.Radius = headDotRadius;
					dot.Visible = true;
				elseif headDots[player.UserId] then
					headDots[player.UserId].Visible = false;
				end
			elseif headDots[player.UserId] then
				headDots[player.UserId].Visible = false;
			end
		end
	end
end);
local Button = MiscTab:CreateButton({[LUAOBFUSACTOR_DECRYPT_STR_0("\147\230\41\163", "\60\221\135\68\198\167")]=LUAOBFUSACTOR_DECRYPT_STR_0("\202\184\235\151\80\214\247\253\203\128\80\208\254\169", "\185\142\221\152\227\34"),[LUAOBFUSACTOR_DECRYPT_STR_0("\123\196\91\246\65\50\244\83", "\151\56\165\55\154\35\83")]=function()
	for _, player in ipairs(Players:GetPlayers()) do
		if (player ~= LocalPlayer) then
			local highlight = player.Character:FindFirstChildOfClass(LUAOBFUSACTOR_DECRYPT_STR_0("\136\74\2\230\172\74\2\230\180", "\142\192\35\101"));
			if highlight then
				highlight:Destroy();
			end
			espenabled = false;
			if drawings[player.UserId] then
				drawings[player.UserId]:Remove();
				drawings[player.UserId] = nil;
			end
			if nameESP[player.UserId] then
				nameESP[player.UserId]:Remove();
				nameESP[player.UserId] = nil;
			end
		end
		for _, dot in pairs(headDots) do
			if dot then
				dot:Remove();
			end
		end
		headDots = {};
		headDotEnabled = false;
		tracerEnabled = false;
		if tracerLines[player.UserId] then
			tracerLines[player.UserId]:Remove();
			tracerLines[player.UserId] = nil;
		end
		AimbotEnabled = false;
		FOVCircle.Visible = false;
		noclipEnabled = false;
		for _, part in pairs(LocalPlayer.Character:GetDescendants()) do
			if (part:IsA(LUAOBFUSACTOR_DECRYPT_STR_0("\244\116\58\166\215\141\190\2", "\118\182\21\73\195\135\236\204")) and (part.CanCollide == false)) then
				part.CanCollide = true;
			end
		end
		WalkSpeedSlider:Set(16);
		JumpPowerSlider:Set(50);
		flying = false;
		if flyConn then
			flyConn:Disconnect();
			flyConn = nil;
		end
		if velocity then
			velocity:Destroy();
			velocity = nil;
		end
		if gyro then
			gyro:Destroy();
			gyro = nil;
		end
		flySpeed = 50;
		if velocity then
			velocity.Velocity = velocity.Velocity.Unit * flySpeed;
		end
		Rayfield:Destroy();
	end
end});

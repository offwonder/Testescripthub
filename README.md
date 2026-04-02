-- Carregar Rayfield
local Rayfield = loadstring(game:HttpGet("https://sirius.menu/rayfield"))()

-- Janela Principal com TEMA CUSTOMIZADO VERMELHO
local Window = Rayfield:CreateWindow({
   Name = "Xitey HUB",
   Icon = 0, -- Mantido em 0 para segurança total
   LoadingTitle = "CARREGANDO Xitey HUB",
   LoadingSubtitle = "criado por: xitey",
   Theme = {
      TextColor = Color3.fromRGB(240, 240, 240),
      Background = Color3.fromRGB(25, 25, 25),
      Topbar = Color3.fromRGB(35, 35, 35),
      Shadow = Color3.fromRGB(15, 15, 15),
      NotificationBackground = Color3.fromRGB(30, 30, 30),
      NotificationActionsBackground = Color3.fromRGB(255, 0, 0), -- Vermelho Puro
      TabBackground = Color3.fromRGB(35, 35, 35),
      TabStroke = Color3.fromRGB(255, 0, 0), -- Bordas em Vermelho
      TabBackgroundSelected = Color3.fromRGB(255, 0, 0), -- Aba selecionada em Vermelho
      TabTextColor = Color3.fromRGB(240, 240, 240),
      SelectedTabTextColor = Color3.fromRGB(255, 255, 255),
      ElementBackground = Color3.fromRGB(35, 35, 35),
      ElementBackgroundHover = Color3.fromRGB(45, 45, 45),
      SecondaryElementBackground = Color3.fromRGB(25, 25, 25),
      ElementStroke = Color3.fromRGB(50, 50, 50),
      SecondaryElementStroke = Color3.fromRGB(40, 40, 40),
      SliderBackground = Color3.fromRGB(255, 0, 0),
      SliderProgress = Color3.fromRGB(255, 0, 0),
      SliderStroke = Color3.fromRGB(255, 50, 50),
      ToggleBackground = Color3.fromRGB(30, 30, 30),
      ToggleEnabled = Color3.fromRGB(255, 0, 0), -- Ativado em Vermelho
      ToggleDisabled = Color3.fromRGB(100, 100, 100),
      ToggleEnabledStroke = Color3.fromRGB(255, 50, 50),
      ToggleDisabledStroke = Color3.fromRGB(125, 125, 125),
      ToggleEnabledOuterStroke = Color3.fromRGB(100, 100, 100),
      ToggleDisabledOuterStroke = Color3.fromRGB(65, 65, 65),
      DropdownSelected = Color3.fromRGB(255, 0, 0),
      DropdownUnselected = Color3.fromRGB(30, 30, 30),
      InputBackground = Color3.fromRGB(30, 30, 30),
      InputStroke = Color3.fromRGB(255, 0, 0),
      PlaceholderColor = Color3.fromRGB(178, 178, 178)
   },
   ToggleUIKeybind = Enum.KeyCode.K,
   ConfigurationSaving = {
      Enabled = true,
      FolderName = "Xitey",
      FileName = "Xitey Hub"
   },
   KeySystem = false
})

-- =========================
-- ABA UNIVERSAL
-- =========================
local UniversalTab = Window:CreateTab("Universal", "home") 

UniversalTab:CreateSection("Scripts Gerais")

UniversalTab:CreateButton({
   Name = "Teddy (Blox Fruits)",
   Callback = function()
      Rayfield:Notify({Title = "Xitey HUB", Content = "Carregando Teddy...", Duration = 3})
      task.spawn(function()
         pcall(function() loadstring(game:HttpGet("https://pastebin.com/raw/dLkdFtJt"))() end)
      end)
   end,
})

-- =========================
-- ABA BLOX FRUITS
-- =========================
local BloxTab = Window:CreateTab("Blox Fruits", "anchor") 

BloxTab:CreateSection("Scripts de Farm & Status")

-- Redz Hub
BloxTab:CreateButton({
   Name = "Redz Hub (Remake)",
   Callback = function()
      Rayfield:Notify({Title = "Xitey HUB", Content = "Iniciando Redz...", Duration = 3})
      local Settings = { JoinTeam = "Pirates"; Translator = true; }
      loadstring(game:HttpGet("https://raw.githubusercontent.com/PlockScripts/newredz/refs/heads/main/Remake-version.luau"))(Settings)
   end,
})

-- BlueX Hub
BloxTab:CreateButton({
   Name = "BlueX Hub",
   Callback = function()
      Rayfield:Notify({Title = "Xitey HUB", Content = "Iniciando BlueX...", Duration = 3})
      _G.AutoTranslate = true 
      _G.SaveConfig = true
      loadstring(game:HttpGet("https://raw.githubusercontent.com/Dev-BlueX/BlueX-Hub/refs/heads/main/Main.lua"))()
   end,
})

-- Quantum Onyx
BloxTab:CreateButton({
   Name = "Quantum Onyx",
   Callback = function()
      Rayfield:Notify({Title = "Xitey HUB", Content = "Iniciando Quantum...", Duration = 3})
      loadstring(game:HttpGet("https://raw.githubusercontent.com/flazhy/QuantumOnyx/refs/heads/main/QuantumOnyx.lua"))()
   end,
})

-- OMG Hub
BloxTab:CreateButton({
   Name = "OMG Hub",
   Callback = function()
      Rayfield:Notify({Title = "Xitey HUB", Content = "Iniciando OMG...", Duration = 3})
      loadstring(game:HttpGet("https://raw.githubusercontent.com/Omgshit/Scripts/main/MainLoader.lua"))()
   end,
})

-- Hoho Hub
BloxTab:CreateButton({
   Name = "Hoho Hub",
   Callback = function()
      Rayfield:Notify({Title = "Xitey HUB", Content = "Iniciando Hoho...", Duration = 3})
      loadstring(game:HttpGet("https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI"))()
   end,
})

-- Bear Hub
BloxTab:CreateButton({
   Name = "Bear Hub",
   Callback = function()
      Rayfield:Notify({Title = "Xitey HUB", Content = "Iniciando Bear...", Duration = 3})
      loadstring(game:HttpGet("https://raw.githubusercontent.com/Huylovemy/Bearhudz/refs/heads/main/Bearhud.lua"))()
   end,
})

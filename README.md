-- Carregar Rayfield
local Rayfield = loadstring(game:HttpGet("https://sirius.menu/rayfield"))()

-- Janela Principal com TEMA CUSTOMIZADO (VERMELHO)
local Window = Rayfield:CreateWindow({
   Name = "Xitey HUB",
   Icon = 0,
   LoadingTitle = "CARREGANDO Xitey HUB",
   LoadingSubtitle = "criado por: xitey",
   Theme = {
      TextColor = Color3.fromRGB(240, 240, 240),

      Background = Color3.fromRGB(25, 25, 25),
      Topbar = Color3.fromRGB(35, 35, 35),
      Shadow = Color3.fromRGB(15, 15, 15),

      NotificationBackground = Color3.fromRGB(30, 30, 30),
      NotificationActionsBackground = Color3.fromRGB(200, 50, 50),

      TabBackground = Color3.fromRGB(35, 35, 35),
      TabStroke = Color3.fromRGB(200, 50, 50), -- Borda da aba em vermelho
      TabBackgroundSelected = Color3.fromRGB(200, 50, 50), -- Aba selecionada em vermelho
      TabTextColor = Color3.fromRGB(240, 240, 240),
      SelectedTabTextColor = Color3.fromRGB(255, 255, 255),

      ElementBackground = Color3.fromRGB(35, 35, 35),
      ElementBackgroundHover = Color3.fromRGB(45, 45, 45),
      SecondaryElementBackground = Color3.fromRGB(25, 25, 25),
      ElementStroke = Color3.fromRGB(50, 50, 50),
      SecondaryElementStroke = Color3.fromRGB(40, 40, 40),

      SliderBackground = Color3.fromRGB(200, 50, 50), -- Slider em vermelho
      SliderProgress = Color3.fromRGB(200, 50, 50),
      SliderStroke = Color3.fromRGB(255, 100, 100),

      ToggleBackground = Color3.fromRGB(30, 30, 30),
      ToggleEnabled = Color3.fromRGB(200, 50, 50), -- Toggle ativado em vermelho
      ToggleDisabled = Color3.fromRGB(100, 100, 100),
      ToggleEnabledStroke = Color3.fromRGB(255, 100, 100),
      ToggleDisabledStroke = Color3.fromRGB(125, 125, 125),
      ToggleEnabledOuterStroke = Color3.fromRGB(100, 100, 100),
      ToggleDisabledOuterStroke = Color3.fromRGB(65, 65, 65),

      DropdownSelected = Color3.fromRGB(200, 50, 50),
      DropdownUnselected = Color3.fromRGB(30, 30, 30),

      InputBackground = Color3.fromRGB(30, 30, 30),
      InputStroke = Color3.fromRGB(200, 50, 50),
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
local UniversalTab = Window:CreateTab("Universal", "globe")

UniversalTab:CreateSection("Scripts Gerais")

UniversalTab:CreateButton({
   Name = "Teddy (Blox Fruits)",
   Callback = function()
      Rayfield:Notify({
         Title = "Xitey HUB",
         Content = "Carregando Teddy Script...",
         Duration = 3
      })
      task.spawn(function()
         pcall(function()
            loadstring(game:HttpGet("https://pastebin.com/raw/dLkdFtJt"))()
         end)
      end)
   end,
})

-- =========================
-- ABA BLOX FRUITS
-- =========================
local BloxTab = Window:CreateTab("Blox Fruits", "swords")

BloxTab:CreateSection("Scripts de Farm & Status")

-- Redz Hub (Remake)
BloxTab:CreateButton({
   Name = "Redz Hub (Remake)",
   Callback = function()
      Rayfield:Notify({
         Title = "Xitey HUB",
         Content = "Iniciando Redz Hub...",
         Duration = 3
      })
      local Settings = {
         JoinTeam = "Pirates"; 
         Translator = true; 
      }
      loadstring(game:HttpGet("https://raw.githubusercontent.com/PlockScripts/newredz/refs/heads/main/Remake-version.luau"))(Settings)
   end,
})

-- 1: BlueX Hub
BloxTab:CreateButton({
   Name = "BlueX Hub",
   Callback = function()
      Rayfield:Notify({
         Title = "Xitey HUB",
         Content = "Iniciando BlueX Hub...",
         Duration = 3
      })
      _G.AutoTranslate = true 
      _G.SaveConfig = true
      loadstring(game:HttpGet("https://raw.githubusercontent.com/Dev-BlueX/BlueX-Hub/refs/heads/main/Main.lua"))()
   end,
})

-- 2: Quantum Onyx
BloxTab:CreateButton({
   Name = "Quantum Onyx",
   Callback = function()
      Rayfield:Notify({
         Title = "Xitey HUB",
         Content = "Iniciando Quantum Onyx...",
         Duration = 3
      })
      loadstring(game:HttpGet("https://raw.githubusercontent.com/flazhy/QuantumOnyx/refs/heads/main/QuantumOnyx.lua"))()
   end,
})

-- 3: OMG Hub
BloxTab:CreateButton({
   Name = "OMG Hub",
   Callback = function()
      Rayfield:Notify({
         Title = "Xitey HUB",
         Content = "Iniciando OMG Hub...",
         Duration = 3
      })
      loadstring(game:HttpGet("https://raw.githubusercontent.com/Omgshit/Scripts/main/MainLoader.lua"))()
   end,
})

-- 4: Hoho Hub
BloxTab:CreateButton({
   Name = "Hoho Hub",
   Callback = function()
      Rayfield:Notify({
         Title = "Xitey HUB",
         Content = "Iniciando Hoho Hub...",
         Duration = 3
      })
      loadstring(game:HttpGet("https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI"))()
   end,
})

-- 5: Bear Hub
BloxTab:CreateButton({
   Name = "Bear Hub",
   Callback = function()
      Rayfield:Notify({
         Title = "Xitey HUB",
         Content = "Iniciando Bear Hub...",
         Duration = 3
      })
      loadstring(game:HttpGet("https://raw.githubusercontent.com/Huylovemy/Bearhudz/refs/heads/main/Bearhud.lua"))()
   end,
})

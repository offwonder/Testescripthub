-- Load XiteyShield
local Rayfield = loadstring(game:HttpGet("https://sirius.menu/rayfield"))()

-- Window
local Window = Rayfield:CreateWindow({
   Name = "Xitey HUB",
   Icon = 0,
   LoadingTitle = "Xitey HUB LOADING",
   LoadingSubtitle = "coded by: xitey",
   Theme = "Red", -- Configurado para Vermelho
   ToggleUIKeybind = Enum.KeyCode.K,

   ConfigurationSaving = {
      Enabled = true,
      FolderName = "Xitey",
      FileName = "Xitey Hub"
   },

   KeySystem = false
})

-- =========================
-- UNIVERSAL TAB
-- =========================
local UniversalTab = Window:CreateTab("Universal", "globe")

UniversalTab:CreateSection("Scripts Universais")

UniversalTab:CreateButton({
   Name = "Teddy (Blox Fruits)",
   Callback = function()
      task.spawn(function()
         pcall(function()
            loadstring(game:HttpGet("https://pastebin.com/raw/dLkdFtJt"))()
         end)
      end)
   end,
})

-- =========================
-- BLOX FRUITS TAB
-- =========================
local BloxTab = Window:CreateTab("Blox Fruits", "swords")

BloxTab:CreateSection("Scripts de Farm & Status")

-- NOVO: Redz Hub (Com Configurações)
BloxTab:CreateButton({
   Name = "Redz Hub (Remake)",
   Callback = function()
      local Settings = {
         JoinTeam = "Pirates"; -- Pirates/Marines
         Translator = true; -- true/false
      }
      loadstring(game:HttpGet("https://raw.githubusercontent.com/PlockScripts/newredz/refs/heads/main/Remake-version.luau"))(Settings)
   end,
})

-- 1: BlueX Hub
BloxTab:CreateButton({
   Name = "BlueX Hub",
   Callback = function()
      _G.AutoTranslate = true 
      _G.SaveConfig = true
      loadstring(game:HttpGet("https://raw.githubusercontent.com/Dev-BlueX/BlueX-Hub/refs/heads/main/Main.lua"))()
   end,
})

-- 2: Quantum Onyx
BloxTab:CreateButton({
   Name = "Quantum Onyx",
   Callback = function()
      loadstring(game:HttpGet("https://raw.githubusercontent.com/flazhy/QuantumOnyx/refs/heads/main/QuantumOnyx.lua"))()
   end,
})

-- 3: OMG Hub
BloxTab:CreateButton({
   Name = "OMG Hub",
   Callback = function()
      loadstring(game:HttpGet("https://raw.githubusercontent.com/Omgshit/Scripts/main/MainLoader.lua"))()
   end,
})

-- 4: Hoho Hub
BloxTab:CreateButton({
   Name = "Hoho Hub",
   Callback = function()
      loadstring(game:HttpGet("https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI"))()
   end,
})

-- 5: Bear Hub
BloxTab:CreateButton({
   Name = "Bear Hub",
   Callback = function()
      loadstring(game:HttpGet("https://raw.githubusercontent.com/Huylovemy/Bearhudz/refs/heads/main/Bearhud.lua"))()
   end,
})

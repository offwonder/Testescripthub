-- Carregar Rayfield
local Rayfield = loadstring(game:HttpGet("https://sirius.menu/rayfield"))()

-- Janela Principal (Resetada para o padrão estável)
local Window = Rayfield:CreateWindow({
   Name = "Xitey HUB",
   Icon = 0, -- Voltamos para 0 para destravar o carregamento
   LoadingTitle = "CARREGANDO Xitey HUB",
   LoadingSubtitle = "criado por: xitey",
   Theme = "Default", -- Tema padrão vermelho da biblioteca
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

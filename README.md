-- Load Rayfield
local Rayfield = loadstring(game:HttpGet("https://sirius.menu/rayfield"))()

-- Window
local Window = Rayfield:CreateWindow({
   Name = "Xitey HUB",
   Icon = 0,
   LoadingTitle = "Xitey HUB LOADING",
   LoadingSubtitle = "coded by: okita",
   Theme = "Ocean",
   ToggleUIKeybind = Enum.KeyCode.K,

   ConfigurationSaving = {
      Enabled = true,
      FolderName = "QIN",
      FileName = "QIN Hub"
   },

   KeySystem = false
})

-- =========================
-- UNIVERSAL TAB
-- =========================
local UniversalTab = Window:CreateTab("Universal", "globe")

UniversalTab:CreateLabel("Universal Script")
UniversalTab:CreateSection("Script universal buatan okita")

-- =========================
-- TEDDY SCRIPT (BLOX FRUITS)
-- =========================
UniversalTab:CreateButton({
   Name = "Teddy (Blox Fruits)",
   Callback = function()
      Rayfield:Notify({
         Title = "QIN HUB",
         Content = "Loading Teddy Script...",
         Duration = 3
      })

      task.spawn(function()
         local success, err = pcall(function()
            loadstring(game:HttpGet(
               "https://pastebin.com/raw/dLkdFtJt"
            ))()
         end)

         if success then
            Rayfield:Notify({
               Title = "QIN HUB",
               Content = "Teddy Script berhasil dimuat",
               Duration = 4
            })
         else
            Rayfield:Notify({
               Title = "Error",
               Content = "Teddy Script gagal dimuat",
               Duration = 5
            })
            warn(err)
         end
      end)
   end,
})

-- =========================
-- GAME TAB
-- =========================

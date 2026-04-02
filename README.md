-- Carregar Rayfield
local Rayfield = loadstring(game:HttpGet("https://sirius.menu/rayfield"))()

-- Janela Principal com o SEU ÍCONE e Tema Vermelho
local Window = Rayfield:CreateWindow({
   Name = "Xitey HUB",
   Icon = 113989457746610, -- Seu Asset ID adicionado aqui!
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
      TabStroke = Color3.fromRGB(200, 50, 50),
      TabBackgroundSelected = Color3.fromRGB(200, 50, 50),
      TabTextColor = Color3.fromRGB(240, 240, 240),
      SelectedTabTextColor = Color3.fromRGB(255, 255, 255),
      ElementBackground = Color3.fromRGB(35, 35, 35),
      ElementBackgroundHover = Color3.fromRGB(45, 45, 45),
      SecondaryElementBackground = Color3.fromRGB(25, 25, 25),
      ElementStroke = Color3.fromRGB(50, 50, 50),
      SecondaryElementStroke = Color3.fromRGB(40, 40, 40),
      SliderBackground = Color3.fromRGB(200, 50, 50),
      SliderProgress = Color3.fromRGB(200, 50, 50),
      SliderStroke = Color3.fromRGB(255, 100, 100),
      ToggleBackground = Color3.fromRGB(30, 30, 30),
      ToggleEnabled = Color3.fromRGB(200, 50, 50),
      ToggleDisabled = Color3.fromRGB(100, 100, 100),
      ToggleEnabledStroke = Color3.fromRGB(255, 100, 100),
      ToggleDisabledStroke = Color3.fromRGB(125, 125, 125),
      ToggleEnabledOuterStroke = Color3.fromRGB(100, 100, 100),
      ToggleDisabledOuterStroke = Color3

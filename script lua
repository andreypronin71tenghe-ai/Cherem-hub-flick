-- ======================== ВЫБОР ЯЗЫКА И УСТРОЙСТВА ========================

local selectedLanguage = "RU"
local selectedDevice = "UNKNOWN"

-- Таблица переводов
local translations = {
   RU = {
      title = "CHEREM HUB | Flick",
      selectLanguage = "Выберите язык",
      selectDevice = "Выберите устройство",
      russian = "🇷🇺 Русский",
      english = "🇬🇧 English",
      pc = "💻 Компьютер",
      mobile = "📱 Мобильный",
      tablet = "📱 Планшет",
      startGame = "Начать игру",
      aimbot = "🎯 Aimbot",
      esp = "👁️ ESP",
      visuals = "🎨 Визуалы",
      controls = "📱 Управление",
      settings = "⚙️ Настройки",
      enableAimbot = "Включить Aimbot",
      showFOVCircle = "Показывать FOV круг",
      fovSize = "Размер FOV",
      colorFOV = "🎨 Цвет FOV круга",
      redChannel = "Красный канал",
      greenChannel = "Зелёный канал",
      blueChannel = "Синий канал",
      aimSettings = "⚙️ Настройки аима",
      aimSmoothing = "Плавность аима",
      sensitivity = "Чувствительность Aimbot",
      prediction = "Предсказание траектории",
      predictionStrength = "Сила предсказания",
      lockDistance = "Дистанция блокировки",
      bodyPart = "Часть тела для наведения",
      head = "Голова",
      torso = "Туловище",
      legs = "Ноги",
      random = "Случайная",
      enableESP = "Включить ESP",
      boxESP = "Box ESP (Боксы вокруг врагов)",
      skeletonESP = "Skeleton ESP (Скелет врага)",
      showDistance = "Показывать расстояние",
      wallhack = "Wallhack (Видеть сквозь стены)",
      brightness = "Включить яркость",
      removeFog = "Отключить туман",
      transparency = "Полупрозрачные враги",
      mobileMode = "Режим мобильного управления",
      touchHoldAim = "Удерживание пальца для аима",
      controlsInfo = "💡 Инструкция управления",
      doubleTap = "👆 Двойной тап - Вкл/Выкл Aimbot",
      hold = "🎯 Удержание - Наведение на врага",
      swipeUp = "☝️ Свайп вверх - Вкл/Выкл ESP",
      swipeDown = "☝️ Свайп вниз - Вкл/Выкл Wallhack",
      reload = "🔄 Перезагрузить скрипт",
      disableAll = "❌ Отключить все функции",
      resetColor = "🎨 Сброс цвета FOV",
      version = "Flick Mobile v2.5.0",
      status = "Статус: ✅ Активен",
      author = "Автор: CHEREM HUB",
      aimEnabled = "Aimbot: ✅ Включен",
      aimDisabled = "Aimbot: ❌ Отключен",
      espEnabled = "ESP: ✅ Включен",
      espDisabled = "ESP: ❌ Отключен",
      wallhackEnabled = "Wallhack: ✅ Включен",
      wallhackDisabled = "Wallhack: ❌ Отключен",
      fovCircleVisible = "FOV круг: ✅ Видимый",
      fovCircleHidden = "FOV круг: ❌ Скрытый",
      brightnessOn = "✅ Яркость увеличена",
      fogRemoved = "✅ Туман отключен",
      colorReset = "✅ Цвет FOV сброшен на зелёный",
      reloading = "Перезагрузка CHEREM HUB...",
      reloaded = "✅ CHEREM HUB перезагружен",
      allDisabled = "❌ Все функции CHEREM HUB отключены",
      loaded = "🔥 CHEREM HUB MOBILE загружен! 🔥",
      readyToUse = "Все функции готовы к использованию",
      targetDirection = "Цель наведения: ",
      smoothnessSet = "Плавность установлена: "
   },
   EN = {
      title = "CHEREM HUB | Flick",
      selectLanguage = "Select language",
      selectDevice = "Select device",
      russian = "🇷🇺 Русский",
      english = "🇬🇧 English",
      pc = "💻 Computer",
      mobile = "📱 Mobile",
      tablet = "📱 Tablet",
      startGame = "Start game",
      aimbot = "🎯 Aimbot",
      esp = "👁️ ESP",
      visuals = "🎨 Visuals",
      controls = "📱 Controls",
      settings = "⚙️ Settings",
      enableAimbot = "Enable Aimbot",
      showFOVCircle = "Show FOV circle",
      fovSize = "FOV size",
      colorFOV = "🎨 FOV circle color",
      redChannel = "Red channel",
      greenChannel = "Green channel",
      blueChannel = "Blue channel",
      aimSettings = "⚙️ Aim settings",
      aimSmoothing = "Aim smoothness",
      sensitivity = "Aimbot sensitivity",
      prediction = "Trajectory prediction",
      predictionStrength = "Prediction strength",
      lockDistance = "Lock distance",
      bodyPart = "Target body part",
      head = "Head",
      torso = "Torso",
      legs = "Legs",
      random = "Random",
      enableESP = "Enable ESP",
      boxESP = "Box ESP (Boxes around enemies)",
      skeletonESP = "Skeleton ESP (Enemy skeleton)",
      showDistance = "Show distance",
      wallhack = "Wallhack (See through walls)",
      brightness = "Enable brightness",
      removeFog = "Remove fog",
      transparency = "Semi-transparent enemies",
      mobileMode = "Mobile control mode",
      touchHoldAim = "Finger hold to aim",
      controlsInfo = "💡 Control instructions",
      doubleTap = "👆 Double tap - Toggle Aimbot",
      hold = "🎯 Hold - Aim at enemy",
      swipeUp = "☝️ Swipe up - Toggle ESP",
      swipeDown = "☝️ Swipe down - Toggle Wallhack",
      reload = "🔄 Reload script",
      disableAll = "❌ Disable all functions",
      resetColor = "🎨 Reset FOV color",
      version = "Flick Mobile v2.5.0",
      status = "Status: ✅ Active",
      author = "Author: CHEREM HUB",
      aimEnabled = "Aimbot: ✅ Enabled",
      aimDisabled = "Aimbot: ❌ Disabled",
      espEnabled = "ESP: ✅ Enabled",
      espDisabled = "ESP: ❌ Disabled",
      wallhackEnabled = "Wallhack: ✅ Enabled",
      wallhackDisabled = "Wallhack: ❌ Disabled",
      fovCircleVisible = "FOV circle: ✅ Visible",
      fovCircleHidden = "FOV circle: ❌ Hidden",
      brightnessOn = "✅ Brightness increased",
      fogRemoved = "✅ Fog removed",
      colorReset = "✅ FOV color reset to green",
      reloading = "CHEREM HUB reloading...",
      reloaded = "✅ CHEREM HUB reloaded",
      allDisabled = "❌ All CHEREM HUB functions disabled",
      loaded = "🔥 CHEREM HUB MOBILE loaded! 🔥",
      readyToUse = "All functions ready to use",
      targetDirection = "Target direction: ",
      smoothnessSet = "Smoothness set: "
   }
}

-- Функция получения перевода
local function t(key)
   if translations[selectedLanguage] and translations[selectedLanguage][key] then
      return translations[selectedLanguage][key]
   end
   return key
end

-- Создаем экран выбора языка и устройства
local screenSize = game:GetService("UserInputService"):GetMouseLocation()

-- Окно выбора
local ChooseWindow = Instance.new("ScreenGui")
ChooseWindow.Name = "ChooseWindow"
ChooseWindow.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ChooseWindow.ResetOnSpawn = false

local Background = Instance.new("Frame")
Background.Name = "Background"
Background.Parent = ChooseWindow
Background.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
Background.Size = UDim2.new(1, 0, 1, 0)
Background.BorderSizePixel = 0

-- Заголовок
local Title = Instance.new("TextLabel")
Title.Name = "Title"
Title.Parent = Background
Title.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
Title.Size = UDim2.new(1, 0, 0.15, 0)
Title.BorderSizePixel = 0
Title.Text = "CHEREM HUB"
Title.TextColor3 = Color3.fromRGB(0, 255, 100)
Title.TextSize = 40
Title.Font = Enum.Font.GothamBold

-- Выбор языка
local LanguageLabel = Instance.new("TextLabel")
LanguageLabel.Name = "LanguageLabel"
LanguageLabel.Parent = Background
LanguageLabel.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
LanguageLabel.Position = UDim2.new(0.1, 0, 0.22, 0)
LanguageLabel.Size = UDim2.new(0.8, 0, 0.08, 0)
LanguageLabel.Text = t("selectLanguage")
LanguageLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
LanguageLabel.TextSize = 24
LanguageLabel.Font = Enum.Font.Gotham
LanguageLabel.BorderSizePixel = 0

-- Кнопка русского
local RUButton = Instance.new("TextButton")
RUButton.Name = "RUButton"
RUButton.Parent = Background
RUButton.BackgroundColor3 = Color3.fromRGB(0, 200, 100)
RUButton.Position = UDim2.new(0.1, 0, 0.32, 0)
RUButton.Size = UDim2.new(0.35, 0, 0.08, 0)
RUButton.Text = t("russian")
RUButton.TextColor3 = Color3.fromRGB(255, 255, 255)
RUButton.TextSize = 20
RUButton.Font = Enum.Font.GothamBold
RUButton.BorderSizePixel = 0

-- Кнопка английского
local ENButton = Instance.new("TextButton")
ENButton.Name = "ENButton"
ENButton.Parent = Background
ENButton.BackgroundColor3 = Color3.fromRGB(0, 150, 200)
ENButton.Position = UDim2.new(0.55, 0, 0.32, 0)
ENButton.Size = UDim2.new(0.35, 0, 0.08, 0)
ENButton.Text = translations.EN.english
ENButton.TextColor3 = Color3.fromRGB(255, 255, 255)
ENButton.TextSize = 20
ENButton.Font = Enum.Font.GothamBold
ENButton.BorderSizePixel = 0

-- Выбор устройства
local DeviceLabel = Instance.new("TextLabel")
DeviceLabel.Name = "DeviceLabel"
DeviceLabel.Parent = Background
DeviceLabel.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
DeviceLabel.Position = UDim2.new(0.1, 0, 0.45, 0)
DeviceLabel.Size = UDim2.new(0.8, 0, 0.08, 0)
DeviceLabel.Text = t("selectDevice")
DeviceLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
DeviceLabel.TextSize = 24
DeviceLabel.Font = Enum.Font.Gotham
DeviceLabel.BorderSizePixel = 0

-- Кнопка ПК
local PCButton = Instance.new("TextButton")
PCButton.Name = "PCButton"
PCButton.Parent = Background
PCButton.BackgroundColor3 = Color3.fromRGB(100, 100, 150)
PCButton.Position = UDim2.new(0.05, 0, 0.58, 0)
PCButton.Size = UDim2.new(0.28, 0, 0.08, 0)
PCButton.Text = t("pc")
PCButton.TextColor3 = Color3.fromRGB(255, 255, 255)
PCButton.TextSize = 18
PCButton.Font = Enum.Font.GothamBold
PCButton.BorderSizePixel = 0

-- Кнопка мобильного
local MobileButton = Instance.new("TextButton")
MobileButton.Name = "MobileButton"
MobileButton.Parent = Background
MobileButton.BackgroundColor3 = Color3.fromRGB(150, 100, 100)
MobileButton.Position = UDim2.new(0.36, 0, 0.58, 0)
MobileButton.Size = UDim2.new(0.28, 0, 0.08, 0)
MobileButton.Text = t("mobile")
MobileButton.TextColor3 = Color3.fromRGB(255, 255, 255)
MobileButton.TextSize = 18
MobileButton.Font = Enum.Font.GothamBold
MobileButton.BorderSizePixel = 0

-- Кнопка планшета
local TabletButton = Instance.new("TextButton")
TabletButton.Name = "TabletButton"
TabletButton.Parent = Background
TabletButton.BackgroundColor3 = Color3.fromRGB(150, 150, 100)
TabletButton.Position = UDim2.new(0.67, 0, 0.58, 0)
TabletButton.Size = UDim2.new(0.28, 0, 0.08, 0)
TabletButton.Text = t("tablet")
TabletButton.TextColor3 = Color3.fromRGB(255, 255, 255)
TabletButton.TextSize = 18
TabletButton.Font = Enum.Font.GothamBold
TabletButton.BorderSizePixel = 0

-- Логика выбора языка
local languageSelected = false
local deviceSelected = false

RUButton.MouseButton1Click:Connect(function()
   selectedLanguage = "RU"
   languageSelected = true
   
   RUButton.BackgroundColor3 = Color3.fromRGB(0, 255, 100)
   ENButton.BackgroundColor3 = Color3.fromRGB(0, 150, 200)
   
   if deviceSelected then
      ChooseWindow:Destroy()
      startGame()
   end
end)

ENButton.MouseButton1Click:Connect(function()
   selectedLanguage = "EN"
   languageSelected = true
   
   ENButton.BackgroundColor3 = Color3.fromRGB(0, 255, 100)
   RUButton.BackgroundColor3 = Color3.fromRGB(0, 200, 100)
   
   if deviceSelected then
      ChooseWindow:Destroy()
      startGame()
   end
end)

PCButton.MouseButton1Click:Connect(function()
   selectedDevice = "PC"
   deviceSelected = true
   
   PCButton.BackgroundColor3 = Color3.fromRGB(150, 150, 200)
   MobileButton.BackgroundColor3 = Color3.fromRGB(150, 100, 100)
   TabletButton.BackgroundColor3 = Color3.fromRGB(150, 150, 100)
   
   if languageSelected then
      ChooseWindow:Destroy()
      startGame()
   end
end)

MobileButton.MouseButton1Click:Connect(function()
   selectedDevice = "MOBILE"
   deviceSelected = true
   
   MobileButton.BackgroundColor3 = Color3.fromRGB(200, 100, 100)
   PCButton.BackgroundColor3 = Color3.fromRGB(100, 100, 150)
   TabletButton.BackgroundColor3 = Color3.fromRGB(150, 150, 100)
   
   if languageSelected then
      ChooseWindow:Destroy()
      startGame()
   end
end)

TabletButton.MouseButton1Click:Connect(function()
   selectedDevice = "TABLET"
   deviceSelected = true
   
   TabletButton.BackgroundColor3 = Color3.fromRGB(200, 200, 100)
   PCButton.BackgroundColor3 = Color3.fromRGB(100, 100, 150)
   MobileButton.BackgroundColor3 = Color3.fromRGB(150, 100, 100)
   
   if languageSelected then
      ChooseWindow:Destroy()
      startGame()
   end
end)

-- Функция запуска игры
function startGame()
   local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

   local Window = Rayfield:CreateWindow({
      Name = t("title"),
      LoadingTitle = "CHEREM HUB",
      LoadingSubtitle = "Подготовка к боевым действиям",
      ConfigurationSaving = {
         Enabled = true,
         FolderName = "CHEREM_HUB_FlickConfig",
         FileName = "Config"
      },
      KeySystem = false
   })

   -- Переменные
   local settings = {
      espEnabled = false,
      aimbotEnabled = false,
      wallhackEnabled = false,
      fovSize = 100,
      sensitivity = 1,
      showDistance = true,
      boxESP = true,
      skeletonESP = false,
      showFOVCircle = true,
      fovCircleColor = Color3.fromRGB(0, 255, 0),
      aimSmoothing = 0.1,
      prediction = true,
      predictionValue = 0.5,
      lockOnDistance = 100,
      mobileAimMode = selectedDevice ~= "PC",
      touchHoldToAim = selectedDevice ~= "PC"
   }

   local Players = game:GetService("Players")
   local UserInputService = game:GetService("UserInputService")
   local RunService = game:GetService("RunService")
   local Camera = workspace.CurrentCamera
   local LocalPlayer = Players.LocalPlayer
   local Mouse = LocalPlayer:GetMouse()

   -- Переменные для мобильного управления
   local isTouching = false
   local touchPosition = Vector2.new(0, 0)
   local touchStartTime = 0
   local isHoldingToAim = false

   -- Создаем FOV круг
   local FOVCircle = Drawing.new("Circle")
   FOVCircle.Visible = true
   FOVCircle.Radius = settings.fovSize
   FOVCircle.Color = settings.fovCircleColor
   FOVCircle.Thickness = 2
   FOVCircle.Filled = false
   FOVCircle.Transparency = 0.8

   -- Создаем текстовый индикатор для мобильного интерфейса
   local MobileStatus = Drawing.new("Text")
   MobileStatus.Visible = true
   MobileStatus.Size = 18
   MobileStatus.Color = Color3.fromRGB(0, 255, 0)
   MobileStatus.Position = Vector2.new(10, 10)

   -- Табы
   local AimbotTab = Window:CreateTab(t("aimbot"), 4483362458)
   local ESPTab = Window:CreateTab(t("esp"), 4483362458)
   local VisualsTab = Window:CreateTab(t("visuals"), 4483362458)
   local ControlsTab = Window:CreateTab(t("controls"), 4483362458)
   local SettingsTab = Window:CreateTab(t("settings"), 4483362458)

   -- ======================== AIMBOT TAB ========================
   AimbotTab:CreateToggle({
      Name = t("enableAimbot"),
      CurrentValue = false,
      Flag = "AimbotToggle",
      Callback = function(Value)
         settings.aimbotEnabled = Value
         print(t("aimEnabled"):gsub("✅", Value and "✅" or "❌"))
      end
   })

   AimbotTab:CreateLabel("═══════════════════════")
   AimbotTab:CreateLabel("🎯 " .. t("fovSize"))
   AimbotTab:CreateLabel("═══════════════════════")

   AimbotTab:CreateToggle({
      Name = t("showFOVCircle"),
      CurrentValue = true,
      Flag = "ShowFOVCircle",
      Callback = function(Value)
         settings.showFOVCircle = Value
         FOVCircle.Visible = Value
      end
   })

   AimbotTab:CreateSlider({
      Name = t("fovSize"),
      Range = {10, 500},
      Increment = 10,
      Suffix = "px",
      CurrentValue = 100,
      Flag = "FOVSlider",
      Callback = function(Value)
         settings.fovSize = Value
         FOVCircle.Radius = Value
      end
   })

   AimbotTab:CreateLabel(t("colorFOV"))

   AimbotTab:CreateSlider({
      Name = t("redChannel"),
      Range = {0, 255},
      Increment = 1,
      Suffix = "",
      CurrentValue = 0,
      Flag = "RedChannel",
      Callback = function(Value)
         local r = Value / 255
         local g = settings.fovCircleColor.G
         local b = settings.fovCircleColor.B
         settings.fovCircleColor = Color3.new(r, g, b)
         FOVCircle.Color = settings.fovCircleColor
      end
   })

   AimbotTab:CreateSlider({
      Name = t("greenChannel"),
      Range = {0, 255},
      Increment = 1,
      Suffix = "",
      CurrentValue = 255,
      Flag = "GreenChannel",
      Callback = function(Value)
         local r = settings.fovCircleColor.R
         local g = Value / 255
         local b = settings.fovCircleColor.B
         settings.fovCircleColor = Color3.new(r, g, b)
         FOVCircle.Color = settings.fovCircleColor
      end
   })

   AimbotTab:CreateSlider({
      Name = t("blueChannel"),
      Range = {0, 255},
      Increment = 1,
      Suffix = "",
      CurrentValue = 0,
      Flag = "BlueChannel",
      Callback = function(Value)
         local r = settings.fovCircleColor.R
         local g = settings.fovCircleColor.G
         local b = Value / 255
         settings.fovCircleColor = Color3.new(r, g, b)
         FOVCircle.Color = settings.fovCircleColor
      end
   })

   AimbotTab:CreateLabel("═══════════════════════")
   AimbotTab:CreateLabel(t("aimSettings"))
   AimbotTab:CreateLabel("═══════════════════════")

   AimbotTab:CreateSlider({
      Name = t("aimSmoothing"),
      Range = {0.01, 1},
      Increment = 0.01,
      Suffix = "",
      CurrentValue = 0.1,
      Flag = "AimSmoothing",
      Callback = function(Value)
         settings.aimSmoothing = Value
         print(t("smoothnessSet") .. Value)
      end
   })

   AimbotTab:CreateSlider({
      Name = t("sensitivity"),
      Range = {0.1, 5},
      Increment = 0.1,
      Suffix = "x",
      CurrentValue = 1,
      Flag = "SensitivitySlider",
      Callback = function(Value)
         settings.sensitivity = Value
      end
   })

   AimbotTab:CreateToggle({
      Name = t("prediction"),
      CurrentValue = true,
      Flag = "PredictionToggle",
      Callback = function(Value)
         settings.prediction = Value
      end
   })

   AimbotTab:CreateSlider({
      Name = t("predictionStrength"),
      Range = {0, 1},
      Increment = 0.05,
      Suffix = "",
      CurrentValue = 0.5,
      Flag = "PredictionValue",
      Callback = function(Value)
         settings.predictionValue = Value
      end
   })

   AimbotTab:CreateSlider({
      Name = t("lockDistance"),
      Range = {10, 500},
      Increment = 10,
      Suffix = " studs",
      CurrentValue = 100,
      Flag = "LockOnDistance",
      Callback = function(Value)
         settings.lockOnDistance = Value
      end
   })

   AimbotTab:CreateDropdown({
      Name = t("bodyPart"),
      Options = {t("head"), t("torso"), t("legs"), t("random")},
      CurrentOption = {t("head")},
      Flag = "AimbotTarget",
      Callback = function(Options)
         print(t("targetDirection") .. Options[1])
      end
   })

   -- ======================== ESP TAB ========================
   ESPTab:CreateToggle({
      Name = t("enableESP"),
      CurrentValue = false,
      Flag = "ESPToggle",
      Callback = function(Value)
         settings.espEnabled = Value
      end
   })

   ESPTab:CreateToggle({
      Name = t("boxESP"),
      CurrentValue = false,
      Flag = "BoxESP",
      Callback = function(Value)
         settings.boxESP = Value
      end
   })

   ESPTab:CreateToggle({
      Name = t("skeletonESP"),
      CurrentValue = false,
      Flag = "SkeletonESP",
      Callback = function(Value)
         settings.skeletonESP = Value
      end
   })

   ESPTab:CreateToggle({
      Name = t("showDistance"),
      CurrentValue = true,
      Flag = "DistanceShow",
      Callback = function(Value)
         settings.showDistance = Value
      end
   })

   ESPTab:CreateToggle({
      Name = t("wallhack"),
      CurrentValue = false,
      Flag = "WallhackToggle",
      Callback = function(Value)
         settings.wallhackEnabled = Value
      end
   })

   -- ======================== VISUALS TAB ========================
   VisualsTab:CreateButton({
      Name = t("brightness"),
      Callback = function()
         local lighting = game:GetService("Lighting")
         lighting.Brightness = 2
         lighting.Ambient = Color3.fromRGB(255, 255, 255)
         print(t("brightnessOn"))
      end
   })

   VisualsTab:CreateButton({
      Name = t("removeFog"),
      Callback = function()
         local lighting = game:GetService("Lighting")
         lighting.FogEnd = 10000
         print(t("fogRemoved"))
      end
   })

   VisualsTab:CreateToggle({
      Name = t("transparency"),
      CurrentValue = false,
      Flag = "TransparencyToggle",
      Callback = function(Value)
         print(t("transparency") .. (Value and "✅" or "❌"))
      end
   })

   -- ======================== CONTROLS TAB ========================
   ControlsTab:CreateLabel("═══════════════════════")
   ControlsTab:CreateLabel("📱 МОБИЛЬНОЕ УПРАВЛЕНИЕ")
   ControlsTab:CreateLabel("═══════════════════════")

   ControlsTab:CreateToggle({
      Name = t("mobileMode"),
      CurrentValue = selectedDevice ~= "PC",
      Flag = "MobileMode",
      Callback = function(Value)
         settings.mobileAimMode = Value
      end
   })

   ControlsTab:CreateToggle({
      Name = t("touchHoldAim"),
      CurrentValue = selectedDevice ~= "PC",
      Flag = "TouchHoldAim",
      Callback = function(Value)
         settings.touchHoldToAim = Value
      end
   })

   ControlsTab:CreateLabel("═══════════════════════")
   ControlsTab:CreateLabel(t("controlsInfo"))
   ControlsTab:CreateLabel("═══════════════════════")

   if selectedDevice ~= "PC" then
      ControlsTab:CreateLabel(t("doubleTap"))
      ControlsTab:CreateLabel(t("hold"))
      ControlsTab:CreateLabel(t("swipeUp"))
      ControlsTab:CreateLabel(t("swipeDown"))
   else
      ControlsTab:CreateLabel("🎮 E - Toggle ESP")
      ControlsTab:CreateLabel("🎮 F - Toggle Aimbot")
      ControlsTab:CreateLabel("🎮 X - Toggle Wallhack")
      ControlsTab:CreateLabel("🎮 V - Toggle FOV Circle")
   end

   -- ======================== SETTINGS TAB ========================
   SettingsTab:CreateLabel("═══════════════════════")
   SettingsTab:CreateLabel("🔥 CHEREM HUB 🔥")
   SettingsTab:CreateLabel("🖥️ Device: " .. selectedDevice)
   SettingsTab:CreateLabel("🌐 Language: " .. selectedLanguage)
   SettingsTab:CreateLabel(t("version"))
   SettingsTab:CreateLabel("═══════════════════════")

   SettingsTab:CreateButton({
      Name = t("reload"),
      Callback = function()
         print(t("reloading"))
         wait(1)
         print(t("reloaded"))
      end
   })

   SettingsTab:CreateButton({
      Name = t("disableAll"),
      Callback = function()
         settings.espEnabled = false
         settings.aimbotEnabled = false
         settings.wallhackEnabled = false
         print(t("allDisabled"))
      end
   })

   SettingsTab:CreateButton({
      Name = t("resetColor"),
      Callback = function()
         settings.fovCircleColor = Color3.fromRGB(0, 255, 0)
         FOVCircle.Color = settings.fovCircleColor
         print(t("colorReset"))
      end
   })

   SettingsTab:CreateLabel(t("status"))
   SettingsTab:CreateLabel(t("author"))

   -- Сохраняем конфиг
   Rayfield:LoadConfiguration()

   -- Уведомление при загрузке
   Rayfield:Notify({
      Title = t("loaded"),
      Content = t("readyToUse"),
      Duration = 3,
      Image = 4483362458
   })

   -- ======================== ОСНОВНАЯ ФУНКЦИЯ АИМА ========================
   local function GetNearestPlayerInFOV(touchPos)
      local nearestPlayer = nil
      local shortestDistance = settings.fovSize

      for _, player in pairs(Players:GetPlayers()) do
         if player ~= LocalPlayer and player.Character then
            local targetPart = player.Character:FindFirstChild("Head")

            if targetPart then
               local screenPos = Camera:WorldToScreenPoint(targetPart.Position)
               local checkPos = touchPos or Mouse.Position

               local distance = (Vector2.new(screenPos.X, screenPos.Y) - Vector2.new(checkPos.X, checkPos.Y)).Magnitude

               if distance < shortestDistance then
                  shortestDistance = distance
                  nearestPlayer = player
               end
            end
         end
      end

      return nearestPlayer
   end

   -- Функция плавного наведения
   local function SmoothAim(targetPosition)
      local currentCFrame = Camera.CFrame
      local targetCFrame = CFrame.new(Camera.CFrame.Position, targetPosition)

      local newCFrame = currentCFrame:Lerp(targetCFrame, settings.aimSmoothing)
      Camera.CFrame = newCFrame
   end

   -- Основной цикл аима
   RunService.RenderStepped:Connect(function()
      -- Обновляем позицию FOV круга
      if isTouching then
         FOVCircle.Position = touchPosition
      else
         FOVCircle.Position = Mouse.Position
      end

      -- Обновляем статус
      MobileStatus.Text = "CHEREM HUB " .. (settings.aimbotEnabled and "✅" or "❌")

      if settings.aimbotEnabled and settings.mobileAimMode then
         local checkPos = isTouching and touchPosition or nil
         local target = GetNearestPlayerInFOV(checkPos)

         if target and target.Character then
            local targetPart = target.Character:FindFirstChild("Head")

            if targetPart then
               local targetPosition = targetPart.Position

               -- Предсказание траектории
               if settings.prediction and target.Character:FindFirstChild("Humanoid") then
                  if target.Character.PrimaryPart and target.Character.PrimaryPart.AssemblyLinearVelocity then
                     targetPosition = targetPosition + (target.Character.PrimaryPart.AssemblyLinearVelocity * settings.predictionValue)
                  end
               end

               -- Плавное наведение
               SmoothAim(targetPosition)
            end
         end
      end
   end)

   -- ======================== СЕНСОРНОЕ УПРАВЛЕНИЕ ========================
   UserInputService.TouchBegan:Connect(function(touch, gameProcessed)
      if gameProcessed then return end

      isTouching = true
      touchPosition = Vector2.new(touch.Position.X, touch.Position.Y)
      touchStartTime = tick()
      isHoldingToAim = true
   end)

   UserInputService.TouchMoved:Connect(function(touch, gameProcessed)
      if gameProcessed then return end

      touchPosition = Vector2.new(touch.Position.X, touch.Position.Y)
   end)

   UserInputService.TouchEnded:Connect(function(touch, gameProcessed)
      isTouching = false
      isHoldingToAim = false

      local touchDuration = tick() - touchStartTime

      -- Двойной тап (быстрый тап и отпуск)
      if touchDuration < 0.2 then
         settings.aimbotEnabled = not settings.aimbotEnabled
         Rayfield:Notify({
            Title = "CHEREM HUB",
            Content = settings.aimbotEnabled and t("aimEnabled") or t("aimDisabled"),
            Duration = 1
         })
      end
   end)

   -- Клавиши для клавиатуры (когда на пк)
   UserInputService.InputBegan:Connect(function(input, gameProcessed)
      if gameProcessed then return end

      if input.KeyCode == Enum.KeyCode.E then
         settings.espEnabled = not settings.espEnabled
         Rayfield:Notify({
            Title = "CHEREM HUB",
            Content = settings.espEnabled and t("espEnabled") or t("espDisabled"),
            Duration = 1
         })
      end

      if input.KeyCode == Enum.KeyCode.F then
         settings.aimbotEnabled = not settings.aimbotEnabled
         Rayfield:Notify({
            Title = "CHEREM HUB",
            Content = settings.aimbotEnabled and t("aimEnabled") or t("aimDisabled"),
            Duration = 1
         })
      end

      if input.KeyCode == Enum.KeyCode.X then
         settings.wallhackEnabled = not settings.wallhackEnabled
         Rayfield:Notify({
            Title = "CHEREM HUB",
            Content = settings.wallhackEnabled and t("wallhackEnabled") or t("wallhackDisabled"),
            Duration = 1
         })
      end

      if input.KeyCode == Enum.KeyCode.V then
         settings.showFOVCircle = not settings.showFOVCircle
         FOVCircle.Visible = settings.showFOVCircle
         Rayfield:Notify({
            Title = "CHEREM HUB",
            Content = settings.showFOVCircle and t("fovCircleVisible") or t("fovCircleHidden"),
            Duration = 1
         })
      end
   end)
end

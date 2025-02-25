-- Script Avançado para Blox Fruits
-- Painel GUI com Várias Funcionalidades

local Library = loadstring(game:HttpGet("https://pastebin.com/raw/wazure"))() -- Carregar Biblioteca GUI (Exemplo)
local Window = Library:CreateWindow("Painel Blox Fruits")

-- Aba Principal
local MainTab = Window:CreateTab("Principal")

-- Botão Farm Automático
MainTab:CreateButton("Farm Automático", function()
    -- Função de farm automático aqui
end)

-- Botão Teleporte
MainTab:CreateButton("Teleporte", function()
    -- Função de teleporte aqui
end)

-- Botão Aumento de XP
MainTab:CreateButton("Aumento de XP", function()
    -- Função de aumento de XP aqui
end)

-- Aba de Configurações
local SettingsTab = Window:CreateTab("Configurações")

-- Botão de Velocidade
SettingsTab:CreateButton("Aumentar Velocidade", function()
    -- Função de aumento de velocidade aqui
end)

-- Slider para Ajuste de Sensibilidade
SettingsTab:CreateSlider("Sensibilidade do Mouse", 1, 100, 50, function(value)
    -- Função de ajuste de sensibilidade aqui
end)

-- Aba de Funções Extra
local ExtrasTab = Window:CreateTab("Extras")

-- Botão de Salto Duplo
ExtrasTab:CreateButton("Salto Duplo", function()
    -- Função de salto duplo aqui
end)

-- Botão de Invisibilidade
ExtrasTab:CreateButton("Invisibilidade", function()
    -- Função de invisibilidade aqui
end)

-- Botão de Energia Infinita
ExtrasTab:CreateButton("Energia Infinita", function()
    -- Função de energia infinita aqui
end)

-- Botão de Fechar/Abrir Painel
local ToggleButton = Instance.new("TextButton")
ToggleButton.Text = "Fechar"
ToggleButton.Position = UDim2.new(0, 10, 0, 10)
ToggleButton.Size = UDim2.new(0, 100, 0, 50)
ToggleButton.MouseButton1Click:Connect(function()
    Window:Toggle() -- Função para abrir/fechar painel
end)

-- Carregar Painel na Tela
screenGui.Parent = game.CoreGui
ToggleButton.Parent = screenGui

print("Painel Blox Fruits Avançado carregado com sucesso.")

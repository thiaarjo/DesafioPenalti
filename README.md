# WallKeeper - Sistema de Simulação de Cobrança de Pênalti (UE5)

O **WallKeeper** é um protótipo de simulação de jogo de futebol focado em mecânicas de cobrança de pênalti, desenvolvido na Unreal Engine 5. O objetivo do projeto é validar a integração de ativos tridimensionais customizados, controle de animações via estados e otimização de cenários complexos para execução em tempo real.

---

## Funcionalidades Implementadas

* **Personagem Goleiro Customizado:** Integração de malha esquelética (Skeletal Mesh) estilizada com aplicação de ativos de animação nativos (`Goalkeeper_Catch_Anim` e estados de repouso).
* **Cenário Otimizado (Craven Cottage):** Integração da estrutura tridimensional do estádio do Fulham via pipeline Fab, utilizando malhas estáticas prontas para jogos (Game Ready Assets) para garantir taxas estáveis de quadros por segundo.
* **Sistema de Visualização:** Configuração de componentes de câmera cinematográfica (`CineCameraActor`) para garantir o enquadramento dinâmico e o rastreamento da área de conversão.

---

## Tecnologias e Ferramentas Utilizadas

* **Motor Gráfico:** Unreal Engine 5
* **Arquitetura de Lógica:** Blueprints Visual Scripting
* **Gerenciamento de Assets:** Epic Games Fab, Sketchfab Pipeline
* **Controle de Versão:** Git com políticas de descarte de arquivos temporários (.gitignore dedicado para Unreal Engine)

---

## Estrutura de Diretórios do Projeto

```text
├── Config/                  # Arquivos de configuração de inicialização e inputs do sistema
├── Content/                 # Ativos de runtime do projeto (Malhas, Materiais e Animações)
│   ├── Blueprints/          # Classe de controle do jogador (BP_ThirdPersonCharacter)
│   ├── CravenCottageStadium/# Ativos tridimensionais estruturais do estádio
│   └── Goalkeeper_skin/     # Malha esquelética, rig e animações do goleiro
└── DesafioPenalti.uproject  # Arquivo descritor do projeto Unreal Engine


Clone Repositorio: https://github.com/thiaarjo/DesafioPenalti
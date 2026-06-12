```markdown
# 🌱 Missão Plante - Sistema Integrado de Rotina Missionária

## 📋 Sobre o Projeto

O **Missão Plante** é um sistema web completo e integrado que combina três ferramentas essenciais para o dia a dia missionário:

- **📋 Rotina Missionária** - Gerenciamento de tarefas diárias, horários e pedidos
- **🌱 Horta** - Planejamento de compras e plantio com calculadora de mudas
- **⏰ Timer + Água** - Automação de horários e monitoramento do tanque

## 🚀 Tecnologias Utilizadas

- HTML5, CSS3 e JavaScript (Vanilla)
- Firebase Realtime Database (backend e sincronização)
- PWA (instalável como aplicativo)
- SortableJS (arrastar para reordenar)
- Canvas API (visualização do tanque)
- Giroscópio (controle por inclinação)

## 🔧 Funcionalidades Completas

### Rotina Missionária
- ✅ Login com múltiplos usuários (admin/missionário)
- ✅ Temas personalizados por usuário (verde, roxo, azul)
- ✅ Lista de tarefas com horários
- ✅ Lista de tarefas essenciais com emojis
- ✅ Sistema de pedidos
- ✅ Progresso visual
- ✅ Adicionar/editar/duplicar/excluir tarefas
- ✅ Arrastar para reordenar
- ✅ Restaurar rotina padrão
- ✅ Cards expansíveis

### Horta
- ✅ Lista de compras por categoria (Folhosas, Raízes, Temperos)
- ✅ Checkboxes sincronizados
- ✅ Tabela de espaçamentos entre plantas
- ✅ Calculadora de mudas (largura × comprimento ÷ espaçamento)
- ✅ Limpar todas as marcações
- ✅ Observações sobre o solo

### Timer + Água
- ✅ Relógio em tempo real
- ✅ Múltiplos timers configuráveis (ON/OFF)
- ✅ Adicionar/remover timers
- ✅ Status LIGADO/DESLIGADO automático
- ✅ Tanque de água com nível ajustável (0-100%)
- ✅ Canvas interativo com bolhas
- ✅ Controle por mouse (movimento horizontal)
- ✅ Suporte a giroscópio (inclinação do telefone)
- ✅ Sincronização em tempo real

## 🔥 Firebase - Estrutura do Banco

```json
{
  "tasks": {
    "{usuario}": {
      "timeline": [...],     // Tarefas com horários
      "extra": [...],        // Tarefas essenciais
      "status": {...}        // Estado das tarefas
    }
  },
  "pedidos": {
    "{usuario}": [...]       // Lista de pedidos
  },
  "users": {
    "{usuario}": {           // Dados de usuário
      "password": "...",
      "role": "admin|executor",
      "theme": "...",
      "name": "...",
      "hasOwnTasks": true
    }
  },
  "horta": {
    "compras": {...}         // Itens da lista de compras
  },
  "timers": {
    "list": [...]            // Configuração dos timers
  },
  "tanque": {
    "nivel": 50              // Nível da água
  }
}
```

👥 Credenciais de Acesso

Usuário Senha Papel Tema
ronan plante Admin Azul
tais planta Admin Roxo
gerardo missionario Admin Verde

📱 Instalação como PWA

1. Abra o aplicativo no navegador
2. Clique no botão "Instalar App" (quando disponível)
3. Ou use a opção "Adicionar à tela inicial" do navegador

🎮 Como Usar

Rotina

1. Faça login com suas credenciais
2. Selecione a pessoa (para admins)
3. Marque as tarefas concluídas
4. Use os botões + para adicionar tarefas
5. Arraste as tarefas para reordenar
6. Clique no cabeçalho dos cards para colapsar/expandir
7. Admins podem adicionar novos usuários

Horta

1. Navegue até a aba "Horta"
2. Marque os itens que já comprou
3. Use a calculadora para planejar quantas mudas cabem
4. Clique em "Limpar todas as marcações" para resetar

Timer + Água

1. Navegue até a aba "Timer + Água"
2. Adicione timers com o botão +
3. Configure os horários de ligar/desligar
4. Ajuste o nível da água com o slider
5. Mova o mouse (ou incline o telefone) para ver o efeito
6. Duplo clique no tanque para nivelar a água

🔒 Recursos de Admin

· Adicionar novos usuários
· Alterar senha de qualquer usuário
· Visualizar todas as rotinas
· Adicionar/remover tarefas de qualquer pessoa

📡 Sincronização

· Tempo real - Todos os dados sincronizam instantaneamente
· Multi-dispositivo - Funciona simultaneamente em vários aparelhos
· Persistente - Dados salvos mesmo fechando o app
· Offline-first - Dados locais sincronizam quando volta online

🛠️ Requisitos Técnicos

· Navegador moderno (Chrome, Firefox, Safari, Edge)
· Conexão com internet (para sincronização)
· HTTPS (obrigatório para PWA e giroscópio)
· Toque ou mouse (para interação)

📦 Estrutura de Arquivos

```
/
├── index.html      # Aplicação completa (este arquivo)
├── manifest.json   # Configuração PWA (embutido)
└── README.txt      # Este arquivo
```

🎯 Melhorias Futuras Possíveis

· Notificações push para lembretes
· Exportar relatórios de progresso
· Gráficos de desempenho semanal
· Compartilhar rotinas entre usuários
· Backup/restore manual
· Autenticação por email/senha do Firebase

🐛 Reportar Problemas

Se encontrar algum bug ou tiver sugestões, entre em contato com o desenvolvedor.

📄 Licença

Uso interno da missão - Todos os direitos reservados.

---

Desenvolvido para facilitar a organização da rotina missionária 🙏

🌱 "Plante boas sementes, colha bons frutos"

```

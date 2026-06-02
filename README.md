# Conference Event Planner 🎯

Um aplicativo web moderno para planejar e calcular despesas de conferências e eventos. Permite selecionar locais, complementos (áudio/vídeo) e refeições, com cálculo automático do custo total. A aplicação foi feita com o auxilio do curso de Desenvolvimento Full-Stack da IBM.

## 📋 Funcionalidades

- **Seleção de Locais**: Escolha entre diferentes salas de conferência com capacidades específicas
- **Complementos (Add-ons)**: Adicione equipamentos audiovisuais como projetores, microfones e palestrantes
- **Seleção de Refeições**: Escolha refeições para o evento e especifique o número de pessoas
- **Cálculo Automático**: Cálculo em tempo real dos custos totais por categoria e valor total
- **Resumo Detalhado**: Visualize um resumo completo de todos os itens selecionados com subtotais
- **Interface Responsiva**: Design intuitivo e fácil de usar

## 🛠️ Tecnologias Utilizadas

- **React** 18+ - Framework JavaScript para construção da UI
- **Redux Toolkit** - Gerenciamento de estado centralizado
- **Vite** - Build tool rápido e moderno
- **CSS3** - Estilos customizados
- **JavaScript ES6+** - Código moderno

## 📦 Estrutura do Projeto

```
src/
├── ConferenceEvent.jsx       # Componente principal
├── TotalCost.jsx             # Componente de resumo de custos
├── AboutUs.jsx               # Página sobre
├── store.js                  # Configuração Redux
├── venueSlice.js             # Redux slice para locais
├── avSlice.js                # Redux slice para complementos
├── mealsSlice.js             # Redux slice para refeições
├── App.jsx                   # Componente raiz
├── App.css                   # Estilos gerais
├── ConferenceEvent.css       # Estilos do componente principal
├── TotalCost.css             # Estilos do resumo
├── main.jsx                  # Ponto de entrada
└── index.css                 # Estilos globais
```

## 🚀 Como Usar

### Instalação

```bash
npm install
```

### Desenvolvimento

```bash
npm run dev
```

Abre a aplicação em modo desenvolvimento. Acesse `http://localhost:5173` no seu navegador.

### Build para Produção

```bash
npm run build
```

### Preview da Build

```bash
npm run preview
```

## 💡 Funcionalidades Detalhadas

### 1. Seleção de Locais
- **Auditorium Hall**: Capacidade para 200 pessoas (máximo 3 unidades)
- **Sala de Conferência**: Configurável com limite de quantidade
- Cada local tem um custo específico

### 2. Complementos
- Projetores ($200)
- Palestrantes ($35)
- Microfones ($45)
- Quadros Brancos ($80)
- Placas de Sinalização ($80)
- Adicione quantidades conforme necessário

### 3. Refeições
- **Café da Manhã** - $50 por pessoa
- **Chá da Tarde** - $25 por pessoa
- **Almoço** - $65 por pessoa
- **Jantar** - $70 por pessoa
- Especifique quantas pessoas serão alimentadas

### 4. Resumo Final
- Visualize todos os itens selecionados em uma tabela
- Veja o custo unitário, quantidade e subtotal de cada item
- Total geral da conferência em destaque

## 🎨 Navegação

- **Barra de Navegação Superior**:
  - Links para "Local", "Complementos" e "Refeições"
  - Botão "Mostrar Detalhes" para ver o resumo final

- **Botões de Ação**:
  - Botões +/- para ajustar quantidades
  - Checkboxes para selecionar refeições
  - Botão "Ver Total Final" ao final da página

## 🔄 Fluxo de Uso

1. Selecione os locais desejados clicando nos botões +/-
2. Adicione complementos audiovisuais necessários
3. Configure o número de pessoas e escolha as refeições
4. Clique em "Mostrar Detalhes" ou "Ver Total Final" para visualizar o resumo
5. Veja o cálculo automático de todos os custos

## 📊 Estado da Aplicação (Redux)

A aplicação usa Redux para gerenciar:
- **venue**: Array de locais com quantidade selecionada
- **av**: Array de complementos com quantidade selecionada
- **meals**: Array de refeições com status de seleção

## 🎯 Próximas Melhorias Sugeridas

- [ ] Persistência de dados (localStorage/sessionStorage)
- [ ] Exportar resumo em PDF
- [ ] Integração com sistema de pagamento
- [ ] Histórico de orçamentos
- [ ] Autenticação de usuários
- [ ] Múltiplos eventos simultâneos

## 📝 Notas

- Os custos são calculados em tempo real
- As mudanças são refletidas imediatamente na interface
- O resumo mostra quantidade e subtotal por item

## 👨‍💻 Autor

Desenvolvido como projeto final IBM ReactProjects

## 📄 Licença

Veja o arquivo LICENSE para detalhes

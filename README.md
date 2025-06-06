# 🤖 Telegram Webhook Manager

Um gerenciador web elegante e intuitivo para webhooks do Telegram Bot API, desenvolvido pela **Techify**.

![Telegram Webhook Manager](https://img.shields.io/badge/Telegram-Bot%20API-blue?style=for-the-badge&logo=telegram)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

## ✨ Funcionalidades

### 🔧 Gerenciamento de Webhook
- **Verificar webhook atual** - Visualize as configurações atuais do seu bot
- **Configurar/Atualizar webhook** - Configure uma nova URL de webhook ou atualize a existente
- **Deletar webhook** - Remova o webhook configurado para receber updates via polling

### 👥 Gerenciamento de Interações
- **Lista de interações recentes** - Visualize usuários, grupos e canais que interagiram com seu bot
- **Envio de mensagens de teste** - Envie mensagens diretamente para testar a comunicação
- **Geração de URLs de teste** - Copie URLs prontas para testar seu bot via API

### 🎨 Interface
- **Design responsivo** - Funciona perfeitamente em desktop, tablet e mobile
- **Interface moderna** - Visual clean com gradientes e efeitos de blur
- **Feedback visual** - Alertas coloridos e estados de loading
- **Ícones Lucide** - Interface rica em ícones vetoriais

## 🚀 Como Usar

### 1. Obtenha seu Token do Bot
1. Abra o Telegram e procure por `@BotFather`
2. Use o comando `/newbot` para criar um novo bot
3. Copie o token fornecido pelo BotFather

### 2. Configure o Webhook (Opcional)
1. Cole seu token do bot no campo correspondente
2. Clique em **"Verificar Webhook"** para ver as configurações atuais
3. Para configurar um novo webhook:
   - Clique em **"Cadastrar/Atualizar"**
   - Insira a URL do seu webhook
   - Clique em **"Salvar Webhook"**

### 3. Teste seu Bot
- Se não houver webhook configurado, você verá uma lista de interações recentes
- Use os botões **"Enviar"** para testar mensagens
- Use **"Copiar URL"** para obter links de teste da API

## 📋 Pré-requisitos

- Navegador web moderno com suporte a:
  - JavaScript ES6+
  - Fetch API
  - CSS Grid e Flexbox
- Token válido de bot do Telegram
- Conexão com a internet

## 🛠️ Instalação

### Opção 1: Download Direto
```bash
# Clone o repositório
git clone https://github.com/seu-usuario/telegram-webhook-manager.git

# Entre no diretório
cd telegram-webhook-manager

# Abra o arquivo HTML no seu navegador
open telegram_webhook_html.html
```

### Opção 2: Hospedagem Web
1. Faça upload do arquivo `telegram_webhook_html.html` para seu servidor web
2. Acesse via browser: `https://seu-dominio.com/telegram_webhook_html.html`

### Opção 3: GitHub Pages
1. Faça fork deste repositório
2. Ative o GitHub Pages nas configurações
3. Acesse via: `https://seu-usuario.github.io/telegram-webhook-manager/`

## 🏗️ Tecnologias Utilizadas

- **HTML5** - Estrutura semântica
- **CSS3** - Estilização moderna com gradientes e backdrop-filter
- **JavaScript (ES6+)** - Lógica da aplicação e integração com API
- **Telegram Bot API** - Comunicação com os serviços do Telegram
- **Lucide Icons** - Biblioteca de ícones vetoriais

## 📱 Responsividade

A aplicação é totalmente responsiva e otimizada para:
- 📱 **Mobile** (< 480px)
- 📱 **Tablet** (480px - 768px)  
- 💻 **Desktop** (> 768px)

## 🔒 Segurança

⚠️ **Importante**: 
- Nunca compartilhe seu token do bot publicamente
- Use conexões HTTPS em produção
- O token é processado apenas no client-side
- Nenhum dado é armazenado em servidores externos

## 🛣️ Roadmap

- [ ] Suporte a múltiplos bots
- [ ] Histórico de mensagens enviadas
- [ ] Templates de mensagens
- [ ] Estatísticas de uso
- [ ] Exportação de dados
- [ ] Tema escuro/claro

## 🤝 Contribuindo

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📝 Exemplo de Uso

```javascript
// Exemplo de integração com webhook
app.post('/webhook', (req, res) => {
  const update = req.body;
  
  if (update.message) {
    const chatId = update.message.chat.id;
    const text = update.message.text;
    
    // Processar mensagem aqui
    console.log(`Mensagem de ${chatId}: ${text}`);
  }
  
  res.sendStatus(200);
});
```

## 🆘 Suporte

Se você encontrar algum problema ou tiver sugestões:

1. Verifique as [Issues existentes](https://github.com/seu-usuario/telegram-webhook-manager/issues)
2. Crie uma nova issue se necessário
3. Consulte a [documentação oficial do Telegram Bot API](https://core.telegram.org/bots/api)

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👨‍💻 Desenvolvido por

**Techify** - Simplificando tecnologia para todos

---

⭐ Se este projeto foi útil para você, considere dar uma estrela no GitHub!

[![GitHub stars](https://img.shields.io/github/stars/seu-usuario/telegram-webhook-manager?style=social)](https://github.com/seu-usuario/telegram-webhook-manager/stargazers)

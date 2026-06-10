# 📚 Repositório de PDFs - NR10

Um site moderno e responsivo para hospedar e gerenciar múltiplos arquivos PDF com facilidade.

## ✨ Funcionalidades

- 🔍 **Busca** - Procure por PDFs por título, descrição ou categoria
- 🎯 **Filtros** - Visualize PDFs recentes, populares ou todos
- 📱 **Responsivo** - Funciona perfeitamente em desktop, tablet e celular
- 👁️ **Visualizador** - Abra PDFs em um modal interativo
- 📥 **Download** - Baixe PDFs diretamente do site
- 🎨 **Design Moderno** - Interface limpa e intuitiva com gradientes e animações

## 🚀 Como Usar

1. **Abrir o site**: Abra `index.html` em seu navegador
2. **Buscar PDFs**: Use a barra de busca para encontrar documentos
3. **Filtrar**: Clique nos botões de filtro (Todos, Recentes, Populares)
4. **Visualizar**: Clique em "Visualizar" para abrir o PDF
5. **Baixar**: Use o botão de download para salvar o PDF

## 📝 Adicionar Novos PDFs

Para adicionar novos PDFs, edite a array `pdfs` no arquivo `index.html`:

```javascript
const pdfs = [
    {
        id: 1,
        titulo: "Título do PDF",
        descricao: "Descrição breve",
        arquivo: "url-da-imagem.jpg",
        url: "link-do-pdf.pdf", // URL do arquivo PDF
        categoria: "Categoria",
        data: "YYYY-MM-DD",
        downloads: 0
    },
    // Adicione mais PDFs...
];
```

### Campos obrigatórios:
- **id**: Número único para cada PDF
- **titulo**: Nome do PDF
- **descricao**: Descrição breve (aparece no card)
- **arquivo**: URL da imagem de capa/thumbnail
- **url**: URL do arquivo PDF para download/visualização
- **categoria**: Categoria do documento
- **data**: Data de adição (formato YYYY-MM-DD)
- **downloads**: Número de downloads (para ordenação)

## 🎯 Exemplo de PDF

```javascript
{
    id: 7,
    titulo: "NR-10 - Segurança em Instalações Elétricas",
    descricao: "Norma reguladora sobre segurança em eletricidade",
    arquivo: "https://via.placeholder.com/400x300?text=NR-10",
    url: "https://example.com/nr10.pdf",
    categoria: "Normas",
    data: "2026-06-10",
    downloads: 150
}
```

## 🛠️ Personalizações

### Mudar cores
Edite as variáveis CSS no arquivo `styles.css`:

```css
:root {
    --primary-color: #2563eb;      /* Azul principal */
    --secondary-color: #1e40af;    /* Azul escuro */
    --accent-color: #f59e0b;       /* Laranja destaque */
    --text-color: #1f2937;         /* Texto */
    --light-bg: #f3f4f6;           /* Fundo claro */
}
```

### Alterar número de colunas
No `styles.css`, procure por:
```css
.pdf-grid {
    grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
}
```

Ajuste o valor `280px` para mais/menos colunas.

## 📊 Estrutura de Arquivos

```
.
├── index.html       # Arquivo principal com HTML e JavaScript
├── styles.css       # Estilos e design responsivo
└── README.md        # Este arquivo
```

## 🌐 Deploy

### GitHub Pages
1. Vá para configurações do repositório
2. Ative GitHub Pages
3. Selecione `main` como branch
4. O site estará disponível em `https://fredparrela.github.io/NR10_update`

### Outras plataformas
- Netlify
- Vercel
- Heroku
- Seu próprio servidor

## 💡 Dicas

- Use URLs válidas para os PDFs (HTTP/HTTPS)
- Crie thumbnails/capas para cada PDF para melhor apresentação
- Organize os PDFs por categoria
- Mantenha as datas atualizadas
- Adicione descrições descritivas para melhor SEO

## 📱 Compatibilidade

- ✅ Chrome/Edge (últimas versões)
- ✅ Firefox (últimas versões)
- ✅ Safari (últimas versões)
- ✅ Mobile (iOS/Android)

## 🔒 Notas de Segurança

- Certifique-se de ter direitos autorais dos PDFs
- Use HTTPS para os links dos arquivos
- Considere adicionar autenticação se necessário

## 📧 Suporte

Para dúvidas ou sugestões, abra uma issue no repositório.

---

**Desenvolvido para facilitar o compartilhamento de documentos NR-10** 📚⚡

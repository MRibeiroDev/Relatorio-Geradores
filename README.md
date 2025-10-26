# **Relatório de Inspeção - Gerador de PDF**

Este projeto é uma aplicação web para geração de relatórios de inspeção de equipamentos, permitindo o preenchimento dinâmico de checklists, inclusão de fotos, assinaturas digitais e exportação do relatório em PDF com layout profissional e controle avançado de quebras de página.

> O sistema utiliza HTML, CSS e JavaScript puro, com as bibliotecas [jsPDF](https://github.com/parallax/jsPDF) e [html2canvas](https://html2canvas.hertzen.com/) para a geração do PDF.

---

## **Pré-requisitos**

1. Navegador moderno (Chrome, Firefox, Edge, etc.)
2. Conexão à internet para carregar as bibliotecas CDN (jsPDF e html2canvas)
3. Não é necessário backend ou instalação local

---

## **Uso**

### 1. Preenchimento do Relatório

- Preencha os dados do equipamento e do responsável.
- Complete os checklists de inspeção, marcando "Conforme", "Não Conforme" ou "N/A".
- Adicione fotos da inspeção (opcional).
- Escreva observações finais.
- Colete assinaturas digitais diretamente na tela.

### 2. Geração do PDF

- Clique no botão **"GERAR RELATÓRIO PDF"**.
- O sistema renderiza cada seção do relatório como imagem, controlando automaticamente as quebras de página para evitar cortes indesejados.
- O PDF é baixado automaticamente com nome personalizado conforme equipamento e data.

---

### **Entradas**

- Dados do equipamento (nome, ativo, marca, modelo, patrimônio)
- Data da inspeção
- Checklists por seção
- Fotos (upload)
- Observações
- Assinaturas digitais

### **Recursos**

- Layout responsivo e pronto para impressão
- Controle avançado de quebra de página no PDF (evita cortes em seções/fotos/assinaturas)
- Assinatura digital via canvas
- Inclusão dinâmica de fotos e legendas
- Barra de progresso por seção
- Exportação em PDF com rodapé automático

---

### **Dependências**

- [jsPDF 2.5.1](https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js)
- [html2canvas 1.4.1](https://cdnjs.cloudflare.com/ajax/libs/html2canvas/1.4.1/html2canvas.min.js)

---

## **Exemplo de Uso**

1. Abra o arquivo `index.html` no navegador.
2. Preencha o relatório conforme necessário.
3. Clique em **"GERAR RELATÓRIO PDF"** para baixar o arquivo.

---

## **Personalização**

- Para alterar os checklists, edite o array `itemsData` no script.
- Para adicionar novos campos ou seções, edite o HTML conforme desejado.

---

## **Licença**

Este projeto é livre para uso e modificação.

---

> [!TIP]
> Para melhor qualidade do PDF, utilize fotos em boa resolução e preencha todos os campos antes de gerar o relatório.

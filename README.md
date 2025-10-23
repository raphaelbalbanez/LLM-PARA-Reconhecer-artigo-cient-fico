🧠 Descrição para o GitHub (README.md)
🧩 Projeto: Sistema de Verificação de Artigos Científicos

Este projeto tem como objetivo analisar documentos (PDF ou imagens) e determinar automaticamente se o arquivo é um artigo científico.
Além disso, o sistema realiza segmentação de texto, contagem de parágrafos, extração de palavras mais frequentes e verificação de conformidade com uma regra simples:

O documento deve ter mais de 2000 palavras e mais de 4 parágrafos.

⚙️ Funcionalidades

🧾 Detecta se o documento parece ser um artigo científico, usando palavras-chave como Resumo, Introdução, Metodologia, Resultados, Conclusão, Referências, DOI, ISSN etc.

🪄 Utiliza técnicas de segmentação para separar o texto:

PDFs: segmentação por blocos de layout com PyMuPDF.

Imagens: segmentação morfológica com OpenCV e OCR por bloco com Tesseract.

📊 Conta parágrafos e palavras e identifica as palavras mais frequentes.

✅ Gera um relatório JSON com todas as informações extraídas.

🤖 O LLM (ChatGPT) é usado apenas para gerar um resumo textual do resultado, cumprindo o requisito de uso mínimo de IA.

🧰 Tecnologias utilizadas

Python 3.10+

PyMuPDF

pdfplumber

OpenCV

pytesseract

Pillow

NumPy

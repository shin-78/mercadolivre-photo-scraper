# MercadoLivre Photo Scraper

Automação em Python para coletar imagens de anúncios do Mercado Livre usando Selenium e exportar para Excel.

---

## Descrição

Este projeto permite coletar fotos grandes de produtos listados em páginas do Mercado Livre.  
Ele percorre anúncios, extrai links das imagens e salva em uma planilha `.xlsx` com o código do anúncio e links das fotos.  

Ideal para análise de produtos, pesquisa de mercado ou backup de imagens.

---

## Estrutura do projeto

mercadolivre-photo-scraper/
├─ src/
│ └─ scraper.py # Código principal do scraper
├─ output/ # Planilhas geradas
├─ run.py # Script para rodar o scraper
├─ requirements.txt # Dependências do projeto
├─ README.md
├─ LICENSE
└─ .gitignore

yaml
Copiar código

---

## Pré-requisitos

- Python 3.10 ou superior
- Google Chrome instalado
- ChromeDriver (gerenciado automaticamente pelo webdriver_manager)
- Bibliotecas Python listadas no `requirements.txt`:

pip install -r requirements.txt

yaml
Copiar código

---

## Como usar

1. Clone o repositório ou faça download:  

git clone https://github.com/seu-usuario/mercadolivre-photo-scraper.git
cd mercadolivre-photo-scraper

csharp
Copiar código

2. Instale as dependências:  

pip install -r requirements.txt

markdown
Copiar código

3. Execute o scraper:  

python run.py

yaml
Copiar código

4. Abra o navegador, faça login no Mercado Livre quando solicitado, e pressione ENTER no terminal.  
5. O script começará a coletar os links e fotos dos anúncios.  
6. A planilha gerada será salva em `output/fotos_mercadolivre.xlsx`.  

---

## Configurações

- **PAUSA**: Intervalo entre carregamento de páginas (em segundos).  
- **LISTA_PAGINAS**: Lista de URLs das páginas do Mercado Livre a serem coletadas.  
- **INICIO**: Número da página a partir da qual começar a coleta (1 = primeira página).  

---

## Observações

- Feche a planilha antes de rodar o script, caso contrário ocorrerá erro ao salvar.  
- É possível adaptar o scraper para outras lojas ou marketplaces alterando os seletores CSS dentro de `scraper.py`.

---

## Licença

Este projeto está sob a licença **MIT**. Consulte o arquivo `LICENSE` para mais informações.

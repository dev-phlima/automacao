# Projeto: Cadastro Automatizado de Produtos

Este projeto tem como objetivo realizar o cadastro automatizado de produtos em um sistema web, utilizando as bibliotecas **PyAutoGUI** e **Pandas**. Ele simula ações humanas no navegador para acessar um sistema, realizar login e preencher formulários com dados extraídos de um arquivo CSV.

---

## Funcionalidades

1. **Abertura Automática do Navegador:**
   - Abre o navegador Google Chrome.
   - Acessa o link do sistema de login.

2. **Login Automático:**
   - Preenche os campos de e-mail e senha.
   - Realiza o login no sistema.

3. **Leitura de Dados de um Arquivo CSV:**
   - Importa os dados do arquivo `produtos.csv` contendo informações sobre os produtos a serem cadastrados.

4. **Cadastro de Produtos:**
   - Preenche automaticamente os campos do formulário com as informações de cada produto.
   - Envia o formulário para cadastrar o produto.
   - Repete o processo até cadastrar todos os produtos da lista.

5. **Ferramenta de Posição de Coordenadas:**
   - O script `pegar_posicao.py` auxilia na captura das coordenadas exatas da tela para cliques e interações.

---

## Estrutura dos Arquivos

- **main.py:** Script principal que executa o fluxo de automação completo.
- **pegar_posicao.py:** Script auxiliar para determinar as coordenadas de cliques e interações na tela.
- **produtos.csv:** Arquivo contendo os dados dos produtos a serem cadastrados, organizado com as seguintes colunas:
  - `codigo`
  - `marca`
  - `tipo`
  - `categoria`
  - `preco_unitario`
  - `custo`
  - `obs`

---

## Pré-requisitos

1. Python 3.8 ou superior.
2. Bibliotecas necessárias (instaláveis via `pip`):
   - `pyautogui`
   - `pandas`
3. Arquivo `produtos.csv` com os dados no mesmo diretório do script principal.

---

## Como Usar

1. **Configurar o Ambiente:**
   - Certifique-se de que o navegador Google Chrome está instalado.
   - Ajuste as coordenadas (x, y) no arquivo `main.py` de acordo com o layout do seu sistema.

2. **Capturar Coordenadas:**
   - Utilize o script `pegar_posicao.py` para obter as coordenadas corretas dos campos e botões no sistema.

3. **Executar o Cadastro:**
   - Execute o script `main.py`:
     ```bash
     python main.py
     ```

---

## Notas

- O sistema automatizado depende de coordenadas específicas para interagir com a interface do usuário. Caso o layout do sistema mude, será necessário atualizar essas coordenadas.
- Recomenda-se rodar o script em um ambiente controlado, pois o PyAutoGUI simula interações humanas diretamente no computador.

--- 

## Autor

Este projeto foi desenvolvido com fins didáticos, baseado em exemplos do curso *Python Impressionador*.

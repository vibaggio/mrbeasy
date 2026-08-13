# mrbeasy

# Facilitador MrBayes 3.2.7a

Uma interface web simplificada para automatizar a configuração, limpeza de dados e execução de análises filogenéticas Bayesianas utilizando o software **MrBayes**. 

Desenvolvida para auxiliar pesquisadores e estudantes a rodarem análises complexas (incluindo o uso de múltiplas threads via MPI no WSL) sem a necessidade de conhecimento prévio em programação ou uso de terminais de comando complexos.

## 🚀 Funcionalidades

* **Conversão Automática:** Transforma arquivos FASTA (`>`) em matrizes NEXUS prontas para o MrBayes.
* **Limpeza e Sanitização:** Remove acentos, caracteres especiais, aspas e cabeçalhos residuais (como os gerados pelo DnaSP) que costumam causar travamentos no MrBayes.
* **Configuração Visual:** Interface amigável para definir o número de gerações, amostragem, variação de taxas e modelo evolutivo (incluindo a inserção de taxas fixas para o modelo GTR).
* **Definição de Outgroup:** Campo dedicado para enraizar a árvore diretamente na execução.
* **Scripts de Execução (1-Click):** Gera automaticamente os arquivos `.bat` para Windows ou comandos diretos para o Ubuntu/WSL. Basta dar dois cliques para a análise iniciar.
* **Instalador Automático:** Script embarcado que configura o Linux (WSL), instala o MrBayes-MPI nativo e baixa a versão Windows automaticamente no computador do usuário.

## 💻 Como Acessar

Você pode utilizar a ferramenta diretamente do seu navegador, sem precisar instalar nada, acessando o link abaixo:

👉 **[Link para a página no GitHub Pages]** *(Substitua aqui pelo link do seu GitHub Pages, ex: https://seu-usuario.github.io/seu-repositorio/)*

Alternativamente, você pode fazer o download do arquivo `index.html` (ou `Interface_MrBayes.html`) deste repositório e dar um duplo clique para rodá-lo offline no seu computador.

## 📖 Como Usar

1. **Instalação Inicial (Apenas na primeira vez):** Se o computador ainda não possui o MrBayes e o Ubuntu/WSL instalados, abra o site e clique em **Baixar Instalador de Dependências**. Execute o arquivo `.bat` gerado como Administrador.
2. **Envio da Matriz:** Arraste e solte o seu arquivo `.fasta` ou `.nexus` na área indicada (ou cole o texto bruto).
3. **Configuração:** Ajuste os parâmetros como número de gerações (ngen), ambiente (Windows ou MPI/Ubuntu) e modelos de substituição.
4. **Geração:** Clique em **Limpar, Processar e Gerar Arquivos**. O navegador fará o download de dois arquivos: o seu arquivo `.nexus` final e o executável de inicialização `.bat`.
5. **Execução:** Coloque os dois arquivos baixados na mesma pasta que contém o `mb.exe` e dê dois cliques no arquivo `.bat`. O terminal abrirá e o processo se iniciará automaticamente.

## ⚠️ Resolução de Problemas Comuns

* **Aviso do Windows Defender ("Não é possível abrir estes arquivos"):** Como o arquivo `.bat` foi gerado no navegador, o Windows pode bloqueá-lo por segurança. Clique com o botão direito no arquivo `.bat` > `Propriedades` > Marque a caixa `Desbloquear` (na parte inferior) > `OK`.
* **Erro de Caminho no MPI:** Certifique-se de não utilizar pastas que contenham espaços no nome ou caracteres especiais para rodar suas análises (ex: evite `C:\Meus Documentos\Análise 1\`, prefira `C:\Analise_1\`).

## ✍️ Autoria e Contato

Ferramenta produzida por **Vinícius Baggio de Souza**.
* 📎 **Currículo Lattes:** [http://lattes.cnpq.br/3742051223020733](http://lattes.cnpq.br/3742051223020733)
* ✉️ **E-mail:** [vinicius.baggio@ufrgs.br](mailto:vinicius.baggio@ufrgs.br)

Projeto vinculado ao **Laboratório de Protozoologia (FAVET - UFRGS)**.
* 📷 **Instagram:** [@protozoovet](https://instagram.com/protozoovet)

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&duration=2500&pause=700&color=2F81F7&center=true&vCenter=true&width=780&lines=%5BSISTEMA%5D+AGENDA+DE+CONTATOS+ONLINE;%5BSISTEMA%5D+CARREGANDO+JSON+%26+MANIPULACAO+DE+ARQUIVOS...;%5BSISTEMA%5D+KWARGS+%26+DICIONARIOS+ATIVOS;%5BSISTEMA%5D+PRONTO+PARA+INTERACAO..." alt="Typing Animation">

<img src="https://capsule-render.vercel.app/api?type=waving&height=160&color=0:05070A,50:0B1F3A,100:061A36&text=AGENDA%20DE%20CONTATOS&fontSize=40&fontColor=E6F1FF&fontAlignY=40&desc=KAIQUE%20JACOB%20%7C%20PYTHON%20%2B%20JSON%20%2B%20MANIPULA%C3%87%C3%83O%20DE%20ARQUIVOS%20%2B%20CLI&descAlignY=65&descSize=15" width="100%" alt="Agenda de Contatos Banner">

</div>

---

<div align="center">

![Python](https://img.shields.io/badge/Python%203.10%2B-0B0F14?style=for-the-badge&logo=python&logoColor=2F81F7)
![JSON](https://img.shields.io/badge/JSON-0B0F14?style=for-the-badge&logo=json&logoColor=2F81F7)
![CLI](https://img.shields.io/badge/Menu%20CLI-0B0F14?style=for-the-badge&logo=gnumeterminal&logoColor=2F81F7)
![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-0B0F14?style=for-the-badge&logo=github&logoColor=2F81F7)

</div>

## `SOBRE`

Sistema interativo de gerenciamento de agenda telefônica e contatos via linha de comando (CLI) desenvolvido em **Python**, focado no domínio de estruturas de dados nativas, modularização de funções e manipulação de arquivos. A aplicação permite o cadastro completo de contatos com múltiplos telefones, e-mails e endereços, além de possibilitar a edição individual de atributos, exibição formatada de relatórios e persistência de dados em arquivos **JSON** e relatórios textuais em **TXT**.

O projeto foi construído para aplicar conceitos essenciais de desenvolvimento em Python, como o uso avançado de dicionários aninhados, tuplas de imutabilidade, desempacotamento de parâmetros variáveis com `**kwargs`, formatação dinâmica de relatórios de texto, além de leitura e escrita com codificação UTF-8 via gerenciadores de contexto (`with open()`).

---

## `CONCEITOS APLICADOS`

```text
AGENDA DE CONTATOS

[✓] Dicionários Aninhados (Estrutura flexível e dinâmica para armazenamento de contatos)
[✓] Tuplas de Imutabilidade (Garantia de tipos de contato suportados no sistema)
[✓] Desempacotamento com **kwargs (Recebimento arbitrário de formas de contato nas funções)
[✓] Manipulação de Arquivos (File I/O nativo com gerenciadores de contexto with open)
[✓] Serialização/Desserialização JSON (Exportação/Importação com json.dumps e json.loads)
[✓] Formatação Dinâmica de Strings (Relatórios tabulados e visualmente limpos via f-strings)
[✓] Separação de Responsabilidades (Funções de regra de dados vs. Funções de I/O com usuário)
[✓] Interface de Terminal CLI (Menu interativo em loop controlado por opções)
[✓] Codificação de Caracteres (Garantia de suporte universal a acentuação com UTF-8)
[✓] Validações Defensivas (Verificação prévia de chaves existentes em coleções)
```

---

## `FUNCIONALIDADES`

| Operação | Descrição |
| --- | --- |
| 👤 Incluir contato | Cadastra um novo contato recebendo dinamicamente múltiplos telefones, e-mails e endereços |
| ➕ Incluir forma de contato | Adiciona novas entradas (ex: um segundo e-mail) a um contato previamente cadastrado |
| ✏️ Alterar nome | Atualiza o identificador do contato mantendo todas as suas formas de comunicação intactas |
| 🔄 Alterar forma de contato | Substitui um valor específico de telefone, e-mail ou endereço por uma nova informação |
| 👁️ Exibir contato | Imprime em tela os dados tabulados e organizados de um único contato especificado |
| 📋 Exibir toda a agenda | Exibe a listagem completa de todos os contatos e seus respectivos meios de comunicação |
| ❌ Excluir contato | Remove o registro e todas as informações vinculadas de um contato da memória |
| 📄 Exportar para TXT | Gera um relatório textual formatado para leitura humana gravado em disco |
| 💾 Exportar para JSON | Serializa a estrutura da agenda em arquivo JSON estruturado mantendo a acentuação |
| 📥 Importar de JSON | Carrega uma agenda armazenada em formato JSON diretamente para a memória da aplicação |

---

## `ESTRUTURA DE DADOS & PERSISTÊNCIA`

* **Estrutura de Memória**: Dicionários aninhados em que a chave principal representa o nome do contato, associada a um dicionário secundário cujas chaves são os meios de comunicação (`telefone`, `email`, `endereco`) mapeando listas de valores:
  ```python
  {
      "Pessoa 1": {
          "telefone": ["11 1234-5678"],
          "email": ["pessoa@email.com", "email@profissional.com"],
          "endereco": ["Rua 123"]
      }
  }
  ```
* **Restrição de Domínio**: A tupla global `contados_suportados` assegura a consistência das chaves aceitas durante o cadastro e atualização de dados.
* **Persistência em JSON**: Utiliza a biblioteca nativa `json` com `indent=4` para legibilidade e `ensure_ascii=False` para preservação nativa da acentuação em português.
* **Exportação Relatorial em TXT**: Monta a saída utilizando a função `agenda_para_texto`, convertendo a estrutura de objetos em linhas delimitadas e tabuladas para relatórios impressos.

---

## `ESTRUTURA DO PROJETO`

```text
sistema-de-agenda/
├── sistema_de_agenda.py
├── agenda_backup.json  (Gerado após exportação/importação)
├── agenda_relatorio.txt (Gerado após exportação em TXT)
├── .gitignore
└── README.md
```

---

## `TECNOLOGIA`

<pre align="center">
[SISTEMA STATUS]

Linguagem  : PYTHON 3.10+
Formato    : JSON / TXT
Interface  : CLI (MENU CONSOLE)
Recursos   : KWARGS / MANIPULAÇÃO DE ARQUIVOS / DICIONÁRIOS ANINHADOS
Status     : CONCLUÍDO

</pre>

<br>
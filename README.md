# 🐚 Shell00 - Basecamp 42

> Objetivo: dominar manipulação de arquivos, permissões e transformação de texto via shell.

---

# Ex00 - Z

## Objetivo
Criar um arquivo que ao usar `cat` mostre:
Z + quebra de linha

## Conceito-chave
- Redirecionamento de saída
- Criação de arquivos simples

## Lógica
Entrada → nada  
Saída → texto fixo dentro de um arquivo

## Insight
Shell também serve pra **gerar conteúdo**, não só executar comandos.

---

# Ex01 - testShell00

## Objetivo
Criar arquivo com permissões específicas e empacotar em `.tar`

## Conceito-chave
- Permissões (`chmod`)
- Estrutura de arquivos
- Compactação

## Ferramentas
- `chmod`
> Controla as permissões de arquivo de **(Usuário, Grupo, Outros)** [rwx]

- `ls -l`
> Lista arquivos de uma pasta atuação ou denominada `-l` faz uma lista longa, mostrando **(Permissões, numero de links, user, group, tamanho dos arquivos, data, nome)**

- `tar`
> Serve para juntar varios arquivos em um só (um "pacote"), arquiva e extrai arquivos usando o comando `tar -cf nome-do-arquivo.tar file1 file2`. Ou extrair um arquivo `tar -xf arquivo.tar`

## Lógica
Criar arquivo → ajustar permissões → validar → compactar 

## Insight
Permissões controlam **quem pode fazer o quê** no sistema.

---

# Ex02 - Estrutura de arquivos

## Objetivo
Reproduzir exatamente uma estrutura com permissões específicas

## Conceito-chave
- Permissões avançadas
- Links simbólicos
- Estrutura de diretórios

## Ferramentas
- `mkdir`
- `touch`
- `chmod`
- `ln -s`

## Lógica
Criar estrutura → ajustar permissões → validar com `ls -l`

## Insight
Você aprende a **replicar ambientes com precisão**.

---

# Ex03 - midLS

## Objetivo
Listar arquivos:
- sem ocultos
- separados por vírgula
- ordenados por tempo

## Conceito-chave
- Manipulação de saída
- Ordenação
- Formatação

## ⚙️ Ferramentas
- `ls`
- flags (`-t`, etc.)

## Lógica
Listar → ordenar → formatar → limpar saída

## Armadilhas
- Mostrar arquivos ocultos
- Formato errado
- Não usar vírgulas

## Insight
Shell = transformar saída até ficar perfeita.

---

# 📌 Ex04 - Git commit

## 🎯 Objetivo
Mostrar os 5 últimos hashes de commit

## 🧠 Conceito-chave
- Histórico do Git
- Filtragem de dados

## ⚙️ Ferramentas
- `git log`
- pipes `|`

## 🔗 Lógica
Extrair commits → filtrar hash → limitar em 5

## ⚠️ Armadilhas
- Mostrar info extra
- Não limitar corretamente

## 💡 Insight
Git funciona como um banco de dados consultável.

---

# 📌 Ex05 - gitignore

## 🎯 Objetivo
Listar arquivos ignorados pelo Git

## 🧠 Conceito-chave
- Controle de versionamento
- Arquivos ignorados

## 🔗 Lógica
Git identifica arquivos ignorados → você extrai essa lista

## ⚠️ Armadilhas
- Misturar com arquivos rastreados
- Formato incorreto

## 💡 Insight
Saber o que **não versionar** é tão importante quanto versionar.

---

# 📌 Ex06 - diff

## 🎯 Objetivo
Gerar diferenças entre arquivos

## 🧠 Conceito-chave
- Comparação de conteúdo
- Patch

## ⚙️ Ferramentas
- `diff`
- `patch`

## 🔗 Lógica
Comparar arquivos → gerar arquivo de diferença

## 💡 Insight
Isso é a base de como Git funciona internamente.

---

# 📌 Ex07 - clean

## 🎯 Objetivo
Encontrar e deletar arquivos específicos

## 🧠 Conceito-chave
- Busca recursiva
- Execução automática

## ⚙️ Ferramentas
- `find`

## 🔗 Lógica
Buscar → filtrar nome → executar ação (delete)

## ⚠️ Armadilhas
- Usar múltiplos comandos (proibido)
- Não deletar de fato

## 💡 Insight
Automação real começa com `find`.

---

# 📌 Ex08 - ft_magic

## 🎯 Objetivo
Criar arquivo que identifica tipo específico de arquivo

## 🧠 Conceito-chave
- Magic numbers
- Identificação de arquivos

## ⚙️ Ferramentas
- `file`

## 🔗 Lógica
Definir regra → sistema reconhece padrão

## 💡 Insight
Arquivos são reconhecidos por conteúdo, não nome.

---

# 🧠 Mentalidade Shell

1. O que entra?
2. O que precisa sair?
3. O que precisa ser transformado?
4. Qual ferramenta faz isso?

---

# 🚀 Conclusão

Shell não é sobre comando.  
É sobre **transformar texto até sobrar só o que você quer**.

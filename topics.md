# Índice

1. [Introdução ao linux](#introdução-ao-linux)
2. [Comandos básicos de navegação](#comandos-básicos-de-navegação)
3. [Criação e gestão de arquivos](#criação-e-gestão-de-arquivos)
4. [Manipulação de arquivos (nano, vim/nvim, emacs)](#manipulação-de-arquivos)
5. Permissões (file permissions, ownership)
6. Filtros e regex (grep, cat, sort, cut, piping/redirection)
7. Gerenciamento de processos
8. Remote shell (SSH)
9. Package manager (apt)
10. Scripting (??)
11. Exercícios práticos
12. Q&A e conclusão (arranjar/fazer cheat sheet)

---
# Introdução ao linux

O linux é um kernel de sistema operativo *open source* que serve como base para diferentes sistemas operativos, desde computadores até televisões e máquinas de café. Foi projetado pelo finlandês Linus Torvalds em 1991 para ser um sistema altamente personalizável.
Entre as características chave do Linux está o facto de ser *open source*, sendo distribuído sob a licensa *GNU General Public License (GPL)*, o que significa que os usuários são livres de utilizar, modificar e distribuir o software para qualquer finalidade, desde que estas modificações também sejam distribuidas com a mesma licensa. Assim, o linux atraiu uma grande comunidade de desenvolvedores e entusiastas da computação, o que levou à rapida evolução deste sistema.

---
# Comandos básicos de navegação

Certamente que uma das primeiras coisas que vos passa pela cabeça ao pensar em usar um terminal é "porquê perder tempo a aprender comandos se podemos fazer tudo através de uma interface gráfica?". E é verdade, quase tudo o que dá para fazer pelos comandos dá para fazer por uma interface gráfica, e o intuito de aprender a utilizar o terminal é complementar a interface gráfica e não substituí-la. Pensem no terminal como mais uma ferramenta para a vossa caixa de ferramentas. Quanto mais completa a caixa de ferramentas, melhor.

Para começar, estes são os comandos básicos de navegação pelas diversas pastas e arquivos do sistema.

| Comando | Descrição | Uso |
| ----------- | ----------- | ----------- |
| pwd | print working directory | pwd |
| man | manual do comando  |   man [command] |
| ls | listar arquivos e pastas | ls [options] [directory] |
| cd | change directory | cd [directory] |

## Caminho relativo vs caminho absoluto

Ao navegar através do terminal um dos conceitos mais importantes é o de caminho relativo e absoluto

### Caminho absoluto

Representa a localização exata do ficheiro/diretório, não dependendo do diretório atual.

Exemplo:

`/home/acm/documentos/workshop.txt`

> Caminhos absolutos começam sempre com `/``.
### Caminho relativo

Representa a localização do ficheiro/diretório em relação ao diretório atual.

Exemplo:

`../downloads/comandos.txt`

#### Ao lidar com caminhos há 3 simbolos que são usados frequentemente:

- `~` : Representa o diretório Home do utilizador atual
  
> `cd ~` ou simplesmente `cd`  leva o utilizador para a pasta Home.
> 
> `cd ~/documentos` refere-se à pasta documentos dentro da paste Home.

- `.` : Representa o diretório atual

> Se a pasta atual é `/home/acm/documentos` então `.` é um *alias*.

- `..` : Representa o diretório acima do atual

> Se a pasta atual é `/home/acm/documentos` então `..` representa `/home/acm` .

##### Através destes comandos é possível navegar livremente por todas as pastas do sistema (desde que o utilizador tenha as permissões necessárias).
---

# Criação e gestão de arquivos

Uma das partes mais importantes de utilizar um terminal é a criação e gestão de arquivos, e estes são os comandos mais utilizados para esse efeito. É necessário ter cuidado ao realizar ações destrutivas (apagar arquivos/pastas) pois não é possível desfazer alterações.

| Comando | Descrição | Uso |
| ----------- | ----------- | ----------- |
| mkdir | criar diretório | mkdir [diretório]|
|touch | criar arquivo | touch [arquivo] |
| rm | apagar arquivo/diretório | rm [options] [file] |
| mv | mover / mudar o nome | mv [source] [destination] |
| cp | copiar | cp [source] [destination] |
---
# Manipulação de arquivos

`WIP`
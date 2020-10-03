# PATTERNS

\# - A cerquilha marca um comentário em nosso arquivo
* - Ignora partes do nome de um pattern, agindo como um coringa
! - Permite que um determinado pattern seja excluído. Geralmente vem acompanhado de outra regra mais genérica
/ - Tem função diferente dependendo da sua localização. No início da linha, ignora um pattern somente naquele diretório, mas não em seus subdiretórios. No final ignora toda a árvore do diretório
\ - A barra invertida atua como um caractere de escape
** - Dois asteriscos em seguida são usados para ignorar um pattern específico dentro de uma árvore de diretórios

Exemplos com patterns:
>Ignora todos os arquivos html do repositório
*.html

>Exceto do arquivo index.html
!index.html

>Ignora o README no diretório atual, mas permite subdir/README
/README

>Ignora todos os arquivos no diretório build/
build/

>Ignora os arquivos .txt do diretório doc/, mas permite subdiretórios (doc/server/arch.txt)
doc/*.txt

>Ignora todos arquivos .pdf na árvore doc/
doc/**/*.pdf
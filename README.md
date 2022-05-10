C:\Users\laris>git config --global user.name "Larissy" C:\Users\laris>git config user.email larissy.s@hotmail.com C:\Users\laris>git config user.name Larissy

tree /f -visualizacao em arvore do diretorio atual

Iniciar repositorio
git init //inicializar repositorio

git status
git -A //trakear todos arquivos
git add readme.md //traker so o aruivo readme.md

C:\Users\laris\Desktop\modulogit\.git>cd .. C:\Users\laris\Desktop\modulogit>git status On branch master No commits yet Untracked files: (use "git add <file>..." to include in what will be committed) README.md nothing added to commit but untracked files present (use "git add" to track) C:\Users\laris\Desktop\modulogit>git add -A C:\Users\laris\Desktop\modulogit>git status On branch master No commits yet Changes to be committed: (use "git rm --cached <file>..." to unstage) new file: README.md C:\Users\laris\Desktop\modulogit>git commit -m "Primeiro commit" [master (root-commit) 69cb4f6] Primeiro commit 1 file changed, 1 insertion(+) create mode 100644 README.md

git commit -m "comentario"

C:\Users\laris\Desktop\modulogit>git commit -m "Criando arquivos index e style, assim como modificando o readme" [master 8e4b1bd] Criando arquivos index e style, assim como modificando o readme 3 files changed, 3 insertions(+), 1 deletion(-) create mode 100644 index.html create mode 100644 style.css C:\Users\laris\Desktop\modulogit>

---

primeiro TRAKEAR
git add -A

depois COMIT
git commit -m "Comentario"
git commit -am "Comentario" /segundo comit

---

COMO REVERTER MODIFICACOES

git log /log de comits

git reset --soft (volta com as modificacoes nao comitadas) --mixed (faz o mesmo mas nao ta comitado, tem que dar o add de novo) --hard (volta td de onde parou) {codigo do comit}

git reset --soft 8e4b1bd10b3519c3bd57c5bf31d066269723dce9

---

BRANCHES

git branch teste //criando branch
git checkout teste //trocando do branch master para o teste

---

SABER O QUE FOI ALTERADO
git status da pra ver o que foi alterado, mas nao da pra ver o q mudou em cada arquivos

git diff //mostra o que foi alterado no arquivo
git diff ---name-only //mostra somente o nome dos arquivos alterados
git diff -style.css //mostra as alterações somente do arquivo style.c/ss
git checkout HEAD(current branch) --style.css //volta pro arquivo
git diff

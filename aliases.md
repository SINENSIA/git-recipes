# 📌 Alias de Git

Los alias en Git permiten definir atajos para comandos largos o repetitivos.

## 📌 Crear alias
```sh
git config --global alias.st "status -sb"
git config --global alias.lg "log --oneline --graph --all --decorate"
git config --global alias.ac "!git add . && git commit -m"
git config --global alias.undo "checkout --"
git config --global alias.uncommit "reset --soft HEAD~1"
```

## 📌 Listar alias configurados
```sh
git config --global --list | grep alias
```


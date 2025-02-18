# ❌ Solución de Problemas en Git

## 📌 Olvidé añadir un archivo al último commit
```sh
git add archivo.txt
git commit --amend --no-edit
```

## 📌 Deshacer `git add` antes del commit
```sh
git reset HEAD archivo.txt
```

## 📌 Revertir un commit sin perder los cambios
```sh
git reset --soft HEAD~1
```

# 📝 Commits y Revertir Cambios

## 📌 Modificar el último commit (mensaje o contenido)
```sh
git commit --amend
```

## 📌 Deshacer el último commit sin perder cambios
```sh
git reset --soft HEAD~1
```

## 📌 Restaurar un archivo a la última versión en remoto
```sh
git checkout origin/main -- archivo.txt
```

# 🔄 Flujos de Trabajo en Git

## 📌 Flujo de trabajo básico con ramas
```sh
git checkout -b feature-nueva
git add .
git commit -m "Agregada nueva funcionalidad"
git push origin feature-nueva
```

## 📌 Rebasing para mantener un historial limpio
```sh
git checkout main
git pull
git checkout feature-nueva
git rebase main
```

# 📋 Instrucciones para el Perfil de GitHub

## 📁 Estructura del Repositorio

```
josemora090525/
├── README.md                          # Perfil principal con estadísticas
├── INSTRUCCIONES.md                   # Este archivo
├── assets/
│   ├── optimus-prime.gif             # GIF de Optimus Prime
│   └── cristiano.gif                 # GIF de Cristiano Ronaldo
└── .github/
    └── workflows/
        ├── update-stats.yml          # Actualización de estadísticas
        └── profile-stats.yml         # Generación de animación de contribuciones
```

## 🤖 Workflows Automáticos

### 1. **Update GitHub Stats** (`update-stats.yml`)
- **Frecuencia**: Cada 6 horas
- **Función**: Actualiza las estadísticas del README automáticamente
- **Ejecución manual**: Ve a Actions → Update GitHub Stats → Run workflow

### 2. **Update Profile Stats** (`profile-stats.yml`)
- **Frecuencia**: Diario (medianoche)
- **Función**: Genera la animación de la serpiente con tus contribuciones
- **Ejecución manual**: Ve a Actions → Update Profile Stats → Run workflow

## 📊 Estadísticas Incluidas

Tu perfil muestra automáticamente:

1. **GitHub Stats**: Total de commits, PRs, issues, estrellas
2. **Streak Stats**: Racha actual y más larga de contribuciones
3. **Top Languages**: Lenguajes más utilizados
4. **Trophies**: Logros de GitHub
5. **Activity Graph**: Gráfico de contribuciones
6. **Snake Animation**: Serpiente que come tus contribuciones

## 🚀 Cómo Usar

### Primera vez (Configuración inicial)

1. **Sube el repositorio a GitHub**:
   ```bash
   git add .
   git commit -m "🎉 Configuración inicial del perfil"
   git push origin main
   ```

2. **Habilita GitHub Actions**:
   - Ve a tu repositorio en GitHub
   - Settings → Actions → General
   - Marca "Allow all actions and reusable workflows"

3. **Configura permisos de workflow**:
   - Settings → Actions → General
   - En "Workflow permissions" selecciona "Read and write permissions"
   - Marca "Allow GitHub Actions to create and approve pull requests"

4. **Ejecuta los workflows manualmente la primera vez**:
   - Ve a la pestaña "Actions"
   - Selecciona "Update Profile Stats"
   - Click en "Run workflow"
   - Espera a que termine (puede tardar 1-2 minutos)

### Actualización automática

Una vez configurado, los workflows se ejecutarán automáticamente:
- **Estadísticas**: Cada 6 horas
- **Animación de serpiente**: Cada día a medianoche

También se actualizarán cada vez que hagas un push al repositorio.

## 🎨 Personalización

### Cambiar tema de las estadísticas

En el `README.md`, puedes cambiar el tema modificando el parámetro `theme`:

```markdown
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=josemora090525&theme=TEMA_AQUI)
```

**Temas disponibles**: 
- `tokyonight` (actual)
- `radical`
- `merko`
- `gruvbox`
- `dark`
- `dracula`
- `monokai`
- `vue`
- `onedark`

### Agregar más GIFs

Simplemente coloca los archivos `.gif` en la carpeta `assets/` y referéncialos en el README:

```markdown
<img src="./assets/tu-gif.gif" width="250" alt="Descripción" />
```

## 🔧 Solución de Problemas

### Los workflows no se ejecutan
- Verifica que GitHub Actions esté habilitado
- Revisa los permisos de workflow (deben ser "Read and write")

### La serpiente no aparece
- Ejecuta manualmente el workflow "Update Profile Stats"
- Espera unos minutos y refresca la página

### Las estadísticas no se actualizan
- Los servicios externos (vercel.app, herokuapp.com) pueden tener caché
- Espera unos minutos o limpia la caché del navegador

## 📝 Notas

- Las estadísticas se actualizan automáticamente, no necesitas hacer nada
- Los commits que hagas en cualquier repositorio se reflejarán en las estadísticas
- La animación de la serpiente se genera en la rama `output` del repositorio

## 🎯 Próximos Pasos

1. Personaliza la sección "Sobre mí" en el README
2. Actualiza el enlace de LinkedIn
3. Agrega más proyectos destacados
4. Personaliza los colores y temas a tu gusto

---

**¡Listo!** Tu perfil de GitHub ahora se actualiza automáticamente con tus estadísticas y contribuciones. 🚀

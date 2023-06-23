1. Abre la terminal y navega hasta el repositorio donde se encuentra el commit que deseas cambiar la fecha.

2. Ejecuta el siguiente comando para abrir el editor de texto predeterminado en Git:

```bash
git rebase -i HEAD~1
```

3. Este comando abre el editor de texto con el último commit en la rama actual. Verás algo como esto:

```bash
pick abcdefg Último commit
```

Cambia la palabra "pick" por "edit" en la línea del commit que deseas cambiar la fecha. Por ejemplo:

```bash
edit abcdefg Último commit
```

4. Guarda y cierra el editor de texto.

5. Ahora, ejecuta el siguiente comando para cambiar la fecha del commit:

```bash
GIT_COMMITTER_DATE="2023-04-21 12:34:56" git commit --amend --no-edit --date "2023-04-21 12:34:45"
```

6. Ejecuta el siguiente comando para continuar con la operación de rebase:

```bash
git rebase --continue
```

7. Finalmente, para actualizarlo en Github:

```bash
git push --force
```

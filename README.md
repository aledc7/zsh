[![aledc.com](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/aledc.com.svg)](https://aledc.com)
[![ingenea.com.ar](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/ingenea.svg)](http://ingenea.com.ar)
[![License](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/mit-license.svg)](https://aledc.com)
[![GitHub release](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/release.svg)](https://aledc.com)
[![Dependencies](https://github.com/aledc7/Scrum-Certification/blob/master/recursos/dependencias-none.svg)](https://aledc.com)


# ZSH -  Personalización


## Agregar nombre de host y usuario al tema predeterminado de ZSH


1. - Primeramente se debe editar el archivo __.zsh__

```js
sudo nano ~/.zshrc
````

2. - Una vez editando este archivo, agregar esta linea al final del mismo

```js
PROMPT='%(!.%{%F{yellow}%}.)$USER @ %{$fg[white]%}%M %{$fg_bold[red]%}➜ %{$fg_bold[green]%}%p %{$fg[cyan]%}%c %{$fg_bold[blue]%}$(git_prompt_info)%{$fg_bold[blue]%} % %{$reset_color%}'
````

3. - Por ultimo salir para reiniciar la terminal, y al ingresar de nuevo, ya tendremos el user y hostname, ademas de seguir conservando la indicacion de ramas de git.



# Poniendo un tema

1. - Descargar el tema de zsh que se quiera de [aca](https://github.com/unixorn/awesome-zsh-plugins#themes)

2. - Copiar el archivo descargado dentro de la carpeta __.oh-my-zsh/templates/__ 
    Los temas en zsh tienen la siguiente nomenclatura:  __nombre.zsh-theme__
    
3. - editar el archivo .zsh y en la variable __ZSH_THEME__ poner el nombre del tema, solo el nombre sin el .zsh-theme

```js
sudo nano ~/.zshrc
````


Luego editar esta linea

```js
ZSH_THEME="agitnoster"
````


eso es todo.








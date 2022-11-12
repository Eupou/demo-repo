# Usando o git

> _Esse repositório tem como objetivo datar o que eu venho aprendendo sobre git e espero que seja util a mais alguém ;)_

<br/>

## Comandos básicos

<br/>

> _Sem esse comandos você não consegue mudar de pasta nem ver os arquivos que tem dentro dela, por isso, esses são os primeiros comandos que você deve entender para que você possa navegar pelas pastas com fluidez._

<br/>

```git
// Utilizado para entrar em uma pasta
$ cd

Input:
suamaquina XXXX ~/Pasta_que_vc_ta
$ cd pasta_super_legal

Output:
suamaquina XXXX ~/Pasta_que_vc_ta/pasta_super_legal
$

---------------------------------

// Volta para a pasta mais a fora
$ cd ..

Input:
suamaquina XXXX ~/Pasta_que_vc_ta/pasta_super_legal
$ cd ..

Output:
suamaquina XXXX ~/Pasta_que_vc_ta
$

---------------------------------

// Lista todos os arquivos dentro de uma pasta
$ dir

Input:
suamaquina XXXX ~/Pasta_que_vc_ta
$ dir

Output:
suamaquina XXXX ~/Pasta_que_vc_ta
$ dir
pasta_super_legal  outra_pasta  fotos_zoadas

    // flag -a, mostra os arquivos que o navegaddor oculta
    ** Supondo que vc tenha iniciado um repositório git

    Input:
    suamaquina XXXX ~/Pasta_que_vc_ta
    $ dir -a

    Output:
    suamaquina XXXX ~/Pasta_que_vc_ta
    $ dir -a
    .  ..  .git  pasta_super_legal  outra_pasta  fotos_zoadas
```

<br/>

## Lidando com pastas e arquivos

> _Com esses comandos você sera capaz de criar pastas e arquivos e também deletá-los_

<br/>

```
// Cria uma nova pasta
$ mkdir

Input:
suamaquina XXXX ~/Pasta_que_vc_ta
$ mkdir pasta_nova

Output:
suamaquina XXXX ~/Pasta_que_vc_ta
$ dir
pasta_nova

    // Lembrando que você pode criar multiplas pastas de uma vez.

    Input:
    suamaquina XXXX ~/Pasta_que_vc_ta
    $ mkdir pasta1  pasta2  pasta3  pastaN

    Output:
    suamaquina XXXX ~/Pasta_que_vc_ta
    $ dir
    pasta1  pasta2  pasta3  pastaN

---------------------------------

// Cria um novo arquivo
$ touch

Input:
suamaquina XXXX ~/Pasta_que_vc_ta
$ touch index.html

Output:
suamaquina XXXX ~/Pasta_que_vc_ta
$ dir
index.html

    // Analogo as pastas você pode criar multiplos arquivos

    Input:
    suamaquina XXXX ~/Pasta_que_vc_ta
    $ touch index.html  styles.css  script.js

    Output:
    suamaquina XXXX ~/Pasta_que_vc_ta
    $ dir
    index.html  styles.css  script.js

// Deleta um arquivo
$ rm nome_do_arquivo.xxxx

Input:
suamaquina XXXX ~/Pasta_que_vc_ta
$ dir
index.html  styles.css  script.js
$ rm index.html

Output:
suamaquina XXXX ~/Pasta_que_vc_ta
$ dir
styles.css  script.js

    // Flag -r, usada para deletar pastas

    ** Lembrando que quando você deleta uma pasta você deleta todos os arquivos e pastas que estiverem dentro dela

    Input:
    suamaquina XXXX ~/Pasta_que_vc_ta
    $ dir
    pasta_que_eu_nao_quero_mais  outra_pasta
    $ rm -r pasta_que_eu_nao_quero_mais

    Output:
    suamaquina XXXX ~/Pasta_que_vc_ta
    $ dir
    outra_pasta

    // Também é possível deletar multiplas pastas e arquivos

    Input:
    suamaquina XXXX ~/Pasta_que_vc_ta
    $ dir
    pasta_chata  pasta_velha  pasta_legal
    $ rm -r pasta_chata pasta_velha

    Output:
    suamaquina XXXX ~/Pasta_que_vc_ta
    $ dir
    pasta_legal

    Input:
    suamaquina XXXX ~/Pasta_que_vc_ta
    $ dir
    oldindex.hml  oldstyles.css  index.html  styles.css
    $ rm -r oldindex.hml oldstyles.css

    Output:
    suamaquina XXXX ~/Pasta_que_vc_ta
    $ dir
    index.html  styles.css
```

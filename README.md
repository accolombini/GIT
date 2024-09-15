### Trabalhando com Git & GitHub

- O propósito desse material é expor um pouco destas ferramentas `git` & `gitHub`
- Para você que está se preparando para o mercado, terá aqui um aliado poderoso
- Para você que está se preparando para seu mestrado/doutorado não precisará se preocupar com seus documentos

Por fim, espero que essas ferramentas sejam um aditivo significativo em sua carreira.

>Bons estudos e divirta-se - assim seu apresndizado será muito mais interessante!!

#### `.gitignore`

- Use para manter arquivos desnecessários fora do repositório.
- Arquivos comuns em `.gitingore`:
  - Arquivos temporários geradps por IDEs (Como PyCharm)
  - Logs, dados de cahce, arquivos de build.
  - Credenciais ou chaves privadas.

#### Plugins interessantes

___Para melhorar a experiência com o Markdown, temos alguns plugins podem ajudar___

    1. Markdown All in One
    2. Markdown Preview Enhanced

##### Alguns comandos que podem ser úteis

    1. Caso queira contar quantos commits foram realizados em seu repositório local use:
      `git rev-list --count HEAD`
    2. Caso queira contar os commits que foram realizados em uma branch específica use:
      `git rev-list --count <nome_da_branch>`
    3. Se quiser saber o número de commits agrupado por autor faça:
      `git shortlog -s`
    4. Se quiser atualizar o repositório local com as mudanças do repositório remoto sem fazer o merge ou modificar seu barnch atual faça:
      `git fetch`
    5. Depois execute o comando a seguir que lhe mostrará se o seu branch local está sincronizado com o branch remoto, use:
      `git status`
    6. Se quiser comparar manualmente os commits entre o repositório local e remoto, use esse comando para visualizar os commits que você tem localmente e que ainda não foram enviados para o repositório remoto:
      `git log origin/main..HEAD --oneline`
    7. Para ver os commits que estão no repositório remoto e que você ainda não puxou para o seu repositório local, use:
      `git log HEAD..origin/main --oneline`
    8. Se você quiser ver exatamente o que mudou entre o seu branch local e o branch remoto, você pode usar:
      `git diff origin/main`
    9. Para trazer os commits remotos que estão faltando no seru repositório local, você pode usar:
      `git pull`

 > __Resumo:__
  git fetch seguido de git status é a maneira mais simples e rápida para verificar se o seu repositório local está sincronizado com o remoto.
  git log origin/main..HEAD mostra os commits que estão localmente e não foram enviados ao remoto.
  git log HEAD..origin/main mostra os commits que estão no remoto e não foram puxados para o local.

##### Atenção:
  >__Para aplicar esses comandos, lembre-se que deve fazer um git fetch antes. Não se esqueça disso, ok!

##### Algo mais para tornar seu arquivo readme.mde mais elegante

1. __Dois subcritos o leva ao negrito__ **Isso também**
2. _Um subcrito o leva ao itálico_ *Isso também*
3. <u>Isso te leva a um sublinhado</u> _Isso é HTML e funciona perfeitamente_
4. ~~Este é um texto riscado~~ em Markdown

---
>__Nota importante:__ `o markdown padrão não suporta listas ordenadas com letras - a. b. c. ... e não suporta texto riscado, esses parâmetros dependem do seu ambiente, o GitHub por exemplo, suporta.
#### Para o PR temos alguns passos a seguir

>Para criar uma nova branch e alternar para ela, o comando é: `git switch -c nome-da-branch`.
>Para alternar entre branches existentes, use: `git switch nome-da-branch-existente`

>Fazer mudanças, adicionar os arquivos e fazer commit: `git add .`
>`git commit -m "Implementa nova funcionalidade"`
>Fazer o push da branch para o repositório remoto:
>`git push origin feature/nova-funcionalidade`

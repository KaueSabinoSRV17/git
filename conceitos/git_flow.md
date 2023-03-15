# Git Flow

Para tornar o processo de desenvolvimento de software algo maduro e eficiente para grandes equipes, 
foi criado o Git Flow. O Git Flow é um padrão de branches fixos.

- main
- development
- feature/<nome-da-feature>
- release/v<número da versão da release>

## Main 

Recebe apenas código pronto para a produção (vindos da `release` ou da `hotfix`). Idealmente cada commit nela gera tags.

## Development

É originada da main. É daqui que saem outras branches para cada feature.

## Feature

É originada da development, e vai conter o trabalho de apenas uma feature específica.

## Release

É originada da development, mas apenas após todas as branches de `feature` forem mergeadas
na `development`. Nela, fazemos o processo de Qualiadade de Software,
onde consertamos bugs apenas relacionados a ela (no caso, os bugs estão em desenvolvimento não em produção).
Estando tudo de acordo, o que está nela é mergeado na main e uma nova versão é gerada.

## HotFix

É originada da main, em ocasiões especiais de bugs em produção. Após o bug ser corrigido,
a branch é mergeada na `main` e na `development`, para que o bug não apareça mais.

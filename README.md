# Marcador de Truco - Android (Kotlin)

Aplicativo nativo Android desenvolvido em **Kotlin** utilizando **Views XML**, **Activities** e **Intents** como atividade avaliativa da Pós-Graduação em Desenvolvimento de Aplicativos Móveis (UTFPR).

## Funcionalidades

- **Contagem de Pontos:** Botões rápidos para somar `+1`, `+3`, `+6`, `+9` e `+12` pontos para cada jogador/equipe.
- **Controle de Partidas:** Ao atingir 12 pontos ou mais, o aplicativo exibe um alerta via `Toast` anunciando o vencedor, contabiliza a vitória no histórico e reinicia o placar da rodada.
- **Histórico de Jogadas (`HistoricoActivity`):** Exibe o total de partidas vencidas por cada jogador/equipe.
- **Personalização de Nomes (`NomesActivity`):** Permite alterar os nomes padrão ("Jogador 1" e "Jogador 2") e atualiza a tela principal via `ActivityResultContracts`.
- **Reiniciar Tudo:** Opção para zerar simultaneamente a pontuação atual, o histórico de vitórias e restaurar os nomes originais.

## Estrutura do Projeto

```text
app/src/main/
├── AndroidManifest.xml
├── java/com/exemplo/marcadortruco/
│   ├── MainActivity.kt
│   ├── HistoricoActivity.kt
│   └── NomesActivity.kt
└── res/layout/
    ├── activity_main.xml
    ├── activity_historico.xml
    └── activity_nomes.xml
```

## Tecnologias Utilizadas

- **Linguagem:** Kotlin
- **Interface (UI):** Android XML Layouts (`LinearLayout`, `TextView`, `Button`, `EditText`)
- **Navegação e Comunicação:** `Intent` explícitas e `ActivityResultLauncher`
- **Feedback Visual:** `Toast`

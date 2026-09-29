# MidgardBrain

[![Build](https://github.com/EduardoPSoares/MidgardBrain/actions/workflows/build.yml/badge.svg)](https://github.com/EduardoPSoares/MidgardBrain/actions/workflows/build.yml)
![Java](https://img.shields.io/badge/Java-21-E76F00?logo=openjdk&logoColor=white)
![Velocity](https://img.shields.io/badge/Velocity-3.3-1BBAE0)
![License](https://img.shields.io/github/license/EduardoPSoares/MidgardBrain)

Plugin Velocity que é a porta de entrada da rede Midgard e a ponte entre o jogo e o
[MidgardBot](https://github.com/EduardoPSoares/MidgardBot) do Discord.

## Destaques

- **Whitelist e vínculo de conta** Discord e Minecraft, com punições aplicadas no login.
- **Fila de entrada** (`/fila`) e **modo manutenção** com agendamento.
- **Sincronização de cargos**: cargos do Discord viram grupos do LuckPerms.
- **Ponte com o bot**: envia eventos ao MidgardBot por socket TCP e recebe mensagens dos servidores por plugin
  messaging.
- Auditoria de ações e dados globais em MySQL ou SQLite (HikariCP).

## Stack

Java 21 · Gradle · Velocity API · LuckPerms API · MySQL/SQLite

## Como compilar

```bash
./gradlew shadowJar
```

O jar sai em `build/libs/`. Configuração em `plugins/MidgardBrain/config.yml`.

# AGENTS.md — Quantaril documentation site

Scope: this repository and every file below it

本repositoryはQuantaril docs projectionでありruntime／protocolの実装正本ではありません。変更前にREADME、MAGI採用票、migration gate、Q Atlantis #19／#28、ZeroRoomLab-manifest公開`main`のAGENTS、SphereOS-Atlantis公開`main`のMAGI bundleと対象Position Skillを読みます。

人間向け文書、Issue、commit、検証報告は日本語を既定とします。MAGIは公開`main`を採用し、`dev`や未merge branchは採用しません。bundleを複製せず、解決したexact SHAを`docs/operations/provenance/`へ記録します。暗黙scan等は自動実行しません。

旧quantaril.cloudはlegacy lineageであり現在仕様へ自動昇格しません。未実装は`NOT_IMPLEMENTED`、未試験は`NOT_TESTED`または`UNKNOWN`、過去OAE不明は`historical-oae-unavailable`です。Q Atlantis #25／#28の承認前にcontentを移植しません。secret等をcommitしません。Docusaurus／deployは#22／#23の別AI scopeです。

最小検証: `git diff --check`と`git status --short --branch`

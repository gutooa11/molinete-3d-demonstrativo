# Contribuição e versionamento
Trabalhar em branches `feat/<issue>-<peca>`, `docs/<issue>-<tema>` ou `fix/<issue>-<problema>`; abrir PR com referência à issue. Commits descritivos em português. Não sobrescrever fonte de outra revisão sem explicar a alteração.

Cada peça tem ID estável P001…; fonte CAD em cad/pecas/<id>, scripts em autocad/pecas/<id>. Usar nomes <id>_<nome>_rNN e unidades mm. Registrar ferramenta/versão, parâmetros consumidos, dependências e passos para regenerar; não declarar compatibilidade AutoCAD ainda não testada. Exportar STEP para sólidos e STL/3MF apenas quando disponíveis, vinculados à revisão fonte. Evitar binários gerados em cada commit; para lotes grandes, usar releases ou avaliar Git LFS.

Parâmetros propostos, medidos e validados devem permanecer distinguíveis. Uma mudança de interface exige revisar ambas as peças, BOM, montagem e ensaios associados. Fonte de verdade inicial: parametros/referencias.json; parâmetros pendentes ficam null, nunca zero artificial.

Antes de concluir: links internos válidos, JSON/CSV legíveis, unidades declaradas, evidência de simulação ou ensaio identificada e nenhuma promessa de funcionalidade sem prova. Não gerar CAD falso para preencher pasta. Registrar decisões em docs/decisoes.md. Tags v0.x para protótipos, sem pressupor liberação física.

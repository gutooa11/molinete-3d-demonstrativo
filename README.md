# Molinete 3D demonstrativo

Projeto decorativo e didático para uma criança de 9 anos, com mecanismos reais: rotor acionado pela manivela, oscilação do carretel, fricção dianteira, antirreverso por catraca/lingueta e arco de fechamento manual. Não destinado à pesca.

**Estado:** organização e especificação inicial. Não há CAD funcional liberado nem validação física nesta base. Pastas de CAD e AutoCAD contêm especificações de trabalho, não modelos fabricáveis.

## Começar
1. Ler [requisitos](docs/requisitos.md), [decisões](docs/decisoes.md) e [interfaces](docs/interfaces.md).
2. Resolver [M0](../../issues/1) e implementar o [esqueleto](../../issues/2).
3. Calibrar [corpos de prova](../../issues/3) antes das peças grandes.
4. Seguir [marcos e tarefas](docs/marcos.md), atualizar [BOM](bom/bom.csv) e registrar evidências.

## Estrutura
- `parametros/`: referências e parâmetros ainda pendentes, em mm.
- `cad/esqueleto/`, `cad/montagem/`: referências comuns e conjunto.
- `cad/pecas/<id>/`: uma pasta por peça, com fonte CAD nativa e exportações quando existirem.
- `autocad/pecas/<id>/`: scripts AutoCAD separados do CAD; versão e execução ainda a definir.
- `impressao/`, `corpos-de-prova/`, `testes/`: perfil inicial e registros.
- `bom/`, `docs/`, `.github/`: compras, arquitetura, contribuição e templates.

## Referências iniciais
Carretel Ø47,5; curso 14,5; relação rotor/manivela 5:1; braço da manivela 55. Esses valores vêm de produtos comerciais diferentes e não comprovam intercambialidade. Não são cotas finais. Excentricidade 7,25 é apenas derivação geométrica para curso simples de 14,5.

Impressão inicial: PETG, bico 0,4 mm. Temperaturas, folgas e demais ajustes dependem da máquina, da bobina e dos corpos de prova. Consulte [impressão](impressao/README.md).

## Histórico e limites
Foram encontrados arquivos locais anteriores com outras hipóteses e perfis PLA. Eles não foram sobrescritos nem publicados como projeto validado. A auditoria e a seleção das revisões a importar estão em #1 e em [inventário](docs/referencias-locais.md).
Licença pendente de decisão do titular; nenhuma licença foi escolhida automaticamente.

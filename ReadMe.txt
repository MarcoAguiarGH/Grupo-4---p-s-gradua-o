| Folder Name | Field Name                   | Field Type | Observation
| FIRES       | Codigo_SGIF                  | Texto      |
| FIRES       | Codigo_ANEPC                 | Numero     |
| FIRES       | Ano                          | Numero     | Tabela DimDate
| FIRES       | Mes                          | Numero     | Tabela DimDate
| FIRES       | Dia                          | Numero     | Tabela DimDate
| FIRES       | Hora                         | Numero     |
| FIRES       | AreaPov                      | Decimal    |
| FIRES       | AreaMato                     | Decimal    |
| FIRES       | AreaAgric                    | Decimal    |
| FIRES       | AreaTotal                    | Decimal    |
| FIRES       | ClasseArea                   | Texto      | range em hectares
| FIRES       | DataHoraAlerta               | TimeStamp  |
| FIRES       | DataHora_PrimeiraIntervencao | TimeStamp  |
| FIRES       | DataHora_Extincao            | TimeStamp  |
| FIRES       | Duracao_Horas                | TimeStamp  |
| FIRES       | IncSup24horas                | Numero     |
| FIRES       | DTCCFR                       | Numero     |
| FIRES       | Distrito                     | Texto      | DimLocation (Distrito)
| FIRES       | Concelho                     | Texto      | DimLocation (Concelho(IdDistrito))
| FIRES       | Freguesia                    | Texto      | DimLocation (Freguesia(IdConcelho))
| FIRES       | Local                        | Texto      | DimLocation (Local(IdFreguesia))
| FIRES       | RNAP                         | Texto      | Transformar noutra tabela ? sigla para (Rede Nacional de Áreas Protegidas)
| FIRES       | RNMNPF                       | Texto      | Transformar noutra tabela ? sigla para (Rede Nacional de Matas Nacionais e Perímetros Florestais)
| FIRES       | X_Militar                    | Numero     | DimLocation ?
| FIRES       | Y_Militar                    | Numero     | DimLocation ?
| FIRES       | Latitude                     | Decimal    | DimLocation ?
| FIRES       | Longitude                    | Decimal    | DimLocation ?
| FIRES       | X_ETRS89                     | Numero     | DimLocation ?
| FIRES       | Y_ETRS89                     | Numero     | DimLocation ?
| FIRES       | DSR                          | Numero     |
| FIRES       | FWI                          | Numero     |
| FIRES       | ISI                          | Numero     |
| FIRES       | DC                           | Numero     |
| FIRES       | DMC                          | Numero     |
| FIRES       | FFMC                         | Numero     |
| FIRES       | BUI                          | Numero     |
| FIRES       | CodCausa                     | Numero     | DimFireCause (ID,TipoCausa,GrupoCausa,DescricaoCausa) Transformar noutra tabela
| FIRES       | TipoCausa                    | Texto      | DimFireCause Transformar noutra tabela
| FIRES       | GrupoCausa                   | Texto      | DimFireType (cada registo deste deve ter um TipoCausa) Transformar noutra tabela
| FIRES       | DescricaoCausa               | Texto      | DimFireType Transformar noutra tabela
| FIRES       | FonteAlerta                  | Texto      | Transformar noutra tabela ? -> DimFireOrigin (renomear tabela para nome mais coerente, já que os dados não satisfazem a ideia original)
| IPMA        | ESTACAO                      | Texto      | DimLocation
| IPMA        | NUM                          | Numero     | ESTACOES.Número
| IPMA        | ANO                          | Numero     | DimDate
| IPMA        | MES                          | Numero     | DimDate
| IPMA        | DIA                          | Numero     | DimDate
| IPMA        | TEMP                         | Decimal    | 
| IPMA        | HR                           | Decimal    | 
| IPMA        | VENTO                        | Decimal    | 
| IPMA        | PREC                         | Decimal    | 
| IPMA        | FFMC                         | Decimal    | 
| IPMA        | DMC                          | Decimal    | 
| IPMA        | DC                           | Decimal    | 
| IPMA        | ISI                          | Decimal    | 
| IPMA        | BUI                          | Decimal    | 
| IPMA        | FWI                          | Decimal    | 
| IPMA        | DSR                          | Decimal    | 
| ESTACOES    | Nome                         | Texto      | 
| ESTACOES    | Número                       | Numero     | IPMA.NUM
| ESTACOES    | Tipo                         | Texto      | Transformar noutra tabela ?
| ESTACOES    | Latitude                     | Decimal    | DimLocation ?
| ESTACOES    | Longitude                    | Decimal    | DimLocation ?
| ESTACOES    | Altitude                     | Decimal    |
| ESTACOES    | Município                    | Texto      | DimLocation (Concelho(IdConcelho))
| ESTACOES    | Início de funcionamento      | Texto      | DimDate ?
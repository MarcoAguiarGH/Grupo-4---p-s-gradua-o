| Folder Name | Field Name                   | Field Type | Observation
| FOGOS       | Codigo_SGIF                  | Texto      |
| FOGOS       | Codigo_ANEPC                 | Numero     |
| FOGOS       | Ano                          | Numero     | Tabela Data
| FOGOS       | Mes                          | Numero     | Tabela Data
| FOGOS       | Dia                          | Numero     | Tabela Data
| FOGOS       | Hora                         | Numero     |
| FOGOS       | AreaPov                      | Decimal    |
| FOGOS       | AreaMato                     | Decimal    |
| FOGOS       | AreaAgric                    | Decimal    |
| FOGOS       | AreaTotal                    | Decimal    |
| FOGOS       | ClasseArea                   | Texto      | range em hectares
| FOGOS       | DataHoraAlerta               | Numero     | Deve ser feito um split de dados
| FOGOS       | DataHora_PrimeiraIntervencao | Numero     | ? tem um formato de hora estranho (time stamp?)
| FOGOS       | DataHora_Extincao            | Numero     | ? tem um formato de hora estranho (time stamp?)
| FOGOS       | Duracao_Horas                | Numero     | ? tem um formato de hora estranho (time stamp?)
| FOGOS       | IncSup24horas                | Numero     |
| FOGOS       | DTCCFR                       | Numero     |
| FOGOS       | Distrito                     | Texto      | tabela DimLocation (Distrito)
| FOGOS       | Concelho                     | Texto      | tabela DimLocation (Concelho(IdDistrito))
| FOGOS       | Freguesia                    | Texto      | tabela DimLocation (Freguesia(IdConcelho))
| FOGOS       | Local                        | Texto      | tabela DimLocation (Local(IdFreguesia))
| FOGOS       | RNAP                         | Texto      | tabela ?, tem dados repetidos logo deve ser uma tabela, mas não sei o que as siglas significam (Rede Nacional de Áreas Protegidas)
| FOGOS       | RNMNPF                       | Texto      | tabela ?, tem dados repetidos logo deve ser uma tabela, mas não sei o que as siglas significam (Rede Nacional de Matas Nacionais e Perímetros Florestais)
| FOGOS       | X_Militar                    | Numero     |
| FOGOS       | Y_Militar                    | Numero     |
| FOGOS       | Latitude                     | Numero     |
| FOGOS       | Longitude                    | Numero     |
| FOGOS       | X_ETRS89                     | Numero     |
| FOGOS       | Y_ETRS89                     | Numero     |
| FOGOS       | DSR                          | Numero     |
| FOGOS       | FWI                          | Numero     |
| FOGOS       | ISI                          | Numero     |
| FOGOS       | DC                           | Numero     |
| FOGOS       | DMC                          | Numero     |
| FOGOS       | FFMC                         | Numero     |
| FOGOS       | BUI                          | Numero     |
| FOGOS       | CodCausa                     | Numero     | tabela DimFireCause (ID,TipoCausa,GrupoCausa,DescricaoCausa)
| FOGOS       | TipoCausa                    | Texto      | tabela DimFireCause
| FOGOS       | GrupoCausa                   | Texto      | tabela DimFireType (cada registo deste deve ter um TipoCausa)
| FOGOS       | DescricaoCausa               | Texto      | tabela DimFireType
| FOGOS       | FonteAlerta                  | Texto      | tabela DimFireOrigin (renomear tabela para nome mais coerente, já que os dados não satisfazem a ideia original)
| IPMA        | ESTACAO                      | Texto      | Tabela DimLocation (Distrito)
| IPMA        | NUM                          | Numero     | Este número é o número da estação
| IPMA        | ANO                          | Numero     | Tabela DimDate
| IPMA        | MES                          | Numero     | Tabela DimDate
| IPMA        | DIA                          | Numero     | Tabela DimDate
| IPMA        | TEMP                         | Numero     | 
| IPMA        | HR                           | Numero     | 
| IPMA        | VENTO                        | Numero     | 
| IPMA        | PREC                         | Numero     | 
| IPMA        | FFMC                         | Numero     | 
| IPMA        | DMC                          | Numero     | 
| IPMA        | DC                           | Numero     | 
| IPMA        | ISI                          | Numero     | 
| IPMA        | BUI                          | Numero     | 
| IPMA        | FWI                          | Numero     | 
| IPMA        | DSR                          | Numero     | 
| ESTACOES    | Nome                         | Texto      | Nome da estação
| ESTACOES    | Número                       | Numero     | Que corresponde ao NUM do ARQ_FWI_OBS_XXXX_REP_CLI.txt
| ESTACOES    | Tipo                         | Texto      | Tabela StationType ? (fazer uma DimTable com esta info?)
| ESTACOES    | Latitude                     | Decimal    |
| ESTACOES    | Longitude                    | Decimal    |
| ESTACOES    | Altitude                     | Decimal    |
| ESTACOES    | Município                    | Texto      | Tabela DimLocation (Concelho(IdConcelho))
| ESTACOES    | Início de funcionamento      | Texto      | Tabela DimDate (precisamos mesmo disto?)
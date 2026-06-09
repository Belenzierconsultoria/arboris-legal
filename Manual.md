# 📖 Manual do Usuário — Arboris

**Versão 1.3.5** · © 2026 Belenzier Consultoria  
*Para uso em campo, 100% offline, Android*

---

## Sumário

1. [Introdução](#1-introdução)
2. [Primeiros Passos](#2-primeiros-passos)
3. [Criando e Gerenciando Projetos](#3-criando-e-gerenciando-projetos)
4. [Métodos de Levantamento](#4-métodos-de-levantamento)
5. [Registrando Indivíduos](#5-registrando-indivíduos)
6. [Banco de Espécies](#6-banco-de-espécies)
7. [Área de Estudo](#7-área-de-estudo)
8. [Mapas e GPS](#8-mapas-e-gps)
9. [Resultados, Cálculos e Gráficos](#9-resultados-cálculos-e-gráficos)
10. [Histórico de Edições](#10-histórico-de-edições)
11. [Relatórios](#11-relatórios)
12. [Central de Exportação](#12-central-de-exportação)
13. [Segurança e Privacidade dos Dados](#13-segurança-e-privacidade-dos-dados)
14. [Perguntas Frequentes (FAQ)](#14-perguntas-frequentes-faq)
15. [Referências Técnicas](#15-referências-técnicas)

---

## 1. Introdução

O Arboris é um aplicativo Android desenvolvido para auxiliar engenheiros florestais, biólogos, técnicos ambientais e consultores na realização de inventários e levantamentos fitossociológicos diretamente em campo, sem necessidade de conexão com a internet para a execução do levantamento florestal.*

> *A conexão com a internet é necessária para o download dos bancos de espécies (recomenda-se fazer previamente ao levantamento) e para visualização da imagem de satélite do mapa, não prejudicando a captura de coordenadas dos indivíduos e dos pontos, ficando este condicionado apenas à capacidade do sinal de GPS do celular.*

### 1.1 O que o Arboris faz

- Registra indivíduos arbóreos com espécie, DAP, CAP, altura, condição e coordenadas GPS
- Suporta 4 métodos de levantamento: Árvores Isoladas, Censo Florestal, Parcelas Fixas e Ponto-Quadrante (PCQM)
- Calcula automaticamente índices fitossociológicos: DA, DR, FA, FR, DoA, DoR, VC%, VI, VIA, Shannon H', Pielou J', Simpson
- Calcula a Suficiência Amostral em tempo real durante o levantamento
- Gera relatórios técnicos em Word (.docx) e PDF prontos para entrega a órgãos ambientais
- Exporta dados em CSV, KML, HTML com gráficos e backup ZIP completo
- Funciona 100% offline — todos os dados ficam armazenados localmente no dispositivo

### 1.2 Planos disponíveis

| Recurso | Plano FREE | Plano PRO |
|---|---|---|
| Projetos | 3 projetos vitalícios | Ilimitados |
| Indivíduos por projeto | Ilimitados | Ilimitados |
| Exportação CSV básica | ✓ | ✓ |
| Cálculos fitossociológicos | — | ✓ |
| Relatório Técnico Word/PDF | — | ✓ |
| Relatório Fotográfico | — | ✓ |
| Gráficos avançados | — | ✓ |
| Backup ZIP completo | — | ✓ |
| Exportação KML e SINAFLOR | — | ✓ |

---

## 2. Primeiros Passos

### 2.1 Instalação

- Baixe o Arboris na Google Play Store buscando por "Arboris Inventário Florestal"
- Abra o aplicativo e leia os Termos de Uso e a Política de Privacidade
- Marque a caixa "Li e aceito" e toque em **Aceitar e Continuar**
- Siga o tutorial inicial (Onboarding) para conhecer as funcionalidades

> ⚠️ **Importante:** Permita o acesso à câmera, galeria e localização GPS quando solicitado. Sem essas permissões, o registro de fotos e coordenadas não funcionará.

### 2.2 Modo Escuro

O Arboris acompanha automaticamente o tema do sistema Android. Para ativar:

- Acesse **Configurações do Android → Tela → Tema Escuro**
- O app mudará para o modo escuro imediatamente

Útil em campo para economia de bateria e melhor visibilidade em ambientes iluminados.

---

## 3. Criando e Gerenciando Projetos

### 3.1 Criar novo projeto

Na tela inicial, toque em **+ Criar Novo Projeto** e preencha:

| Campo | Descrição | Obrigatório |
|---|---|---|
| Nome do Projeto | Identificação do levantamento | Sim |
| Descrição | Observações gerais | Não |
| Cliente | Nome do proprietário ou contratante | Não |
| Responsável Técnico | Engenheiro ou biólogo responsável | Não |
| Município/Estado | Localização do empreendimento | Não |
| Método de Levantamento | Ver seção 4 | Sim |

> 💡 **Dica:** O método de levantamento não pode ser alterado após a criação do projeto. Escolha com atenção antes de confirmar.

### 3.2 Tela principal do projeto (Hub)

Após criar ou abrir um projeto, você acessa o **Hub Central** com as seções:

- **Levantamento Fitossociológico** — Acesso direto ao registro de indivíduos
- **Configurações do Projeto** (DAP mínimo, fator forma, fator de conversão e área total)
- **Área de Estudo**
- **Banco de Espécies**
- **Bancos por Fitofisionomia** (o download dos bancos de espécies requer conexão com a internet)
- **Análise** — Resultados, Configurações do projeto, Relatórios Word/PDF, Exportação
- **Visualização** — Mapa Interativo, Pontos de Interesse, Gráficos

### 3.3 Configurações do projeto

Acesse **Hub → Configurações do Projeto** para ajustar:

| Parâmetro | Padrão | Descrição |
|---|---|---|
| DAP Mínimo de Inclusão | 5,0 cm | Indivíduos abaixo deste valor são excluídos dos cálculos |
| Fator de Forma | 0,7 | Coeficiente para cálculo de volume (cilindro parabólico) |
| Fator de Conversão | 1,4 | Conversão de volume sólido (m³) para estéreo (mst) |
| Área Total (ha) | — | Obrigatório para Censo Florestal |

---

## 4. Métodos de Levantamento

### 4.1 Árvores Isoladas

Indicado para supressão de árvores individuais (licenciamento ambiental). Cada indivíduo é registrado individualmente sem vínculo a parcelas.

- Acesse: **Hub → Levantamento Fitossociológico → lista de indivíduos**
- Registre DAP (via CAP), altura, espécie e condição (Viva/Morta)
- Capture GPS de cada indivíduo para georreferenciamento
- Exporta planilha SINAFLOR no formato exato de importação do sistema federal

### 4.2 Censo Florestal

Inventário 100% de uma área definida. Todos os indivíduos com DAP ≥ DAP mínimo são registrados.

- Configure a **Área Total (ha)** em Configurações do Projeto antes de começar
- Registre todos os indivíduos na lista principal
- Gera densidade, área basal e volume por hectare

### 4.3 Parcelas Fixas

Método de amostragem por unidades fixas. Recomendado para inventários de fragmentos florestais.

- Crie as parcelas em **Hub → Levantamento → Lista de Parcelas**
- Informe o número, tamanho (m²) e capture as coordenadas GPS de cada parcela
- Toque em uma parcela para abrir a lista de indivíduos daquela parcela
- Registre os indivíduos normalmente

Os resultados incluem Estatística Amostral (ACS) com coeficiente de variação, erro relativo e suficiência amostral.

### 4.4 Ponto-Quadrante (PCQM)

Método de distância para estimativa de densidade. Cada ponto amostral possui 4 quadrantes.

- Crie os pontos em **Hub → Levantamento → Lista de Pontos**
- Para cada ponto, acesse os **Quadrantes** e registre 1 indivíduo por quadrante
- Informe a distância do ponto ao indivíduo mais próximo em cada quadrante

A densidade é estimada com base nas distâncias registradas, sem necessidade de definir área total.

---

## 5. Registrando Indivíduos

### 5.1 Campos do formulário

| Campo | Descrição | Obrigatório |
|---|---|---|
| Número | Gerado automaticamente ou manual | Sim |
| Espécie | Busca por nome científico, comum, ou família | Sim |
| Número de Fustes | 1 a 4 fustes por indivíduo | Sim |
| CAP (cm) | Circunferência à Altura do Peito — DAP calculado automaticamente | Sim |
| Altura (m) | Altura total do indivíduo | Sim |
| Condição | Viva ou Morta | Sim |
| Distância (m) | Apenas para Ponto-Quadrante | Situacional |
| Fotos | Câmera ou galeria | Não |
| GPS | Capturado automaticamente ao abrir o formulário | Não |
| Observações | Anotações livres | Não |

### 5.2 Busca de espécies

Digite pelo menos 2 caracteres do nome científico, nome comum ou família para buscar no banco de espécies. Opções especiais:

- ❓ **Não Identificado** — registra sem vínculo a espécie
- 🔄 **Repetir Espécie** — repete a última espécie registrada no projeto (agiliza trabalho em campo)

### 5.3 Indivíduos com múltiplos fustes

Para árvores bifurcadas, selecione o número de fustes (2, 3 ou 4). O DAP equivalente é calculado automaticamente pela soma das áreas basais de todos os fustes.

### 5.4 Validação inteligente

O app alerta automaticamente quando detecta valores suspeitos:

- DAP abaixo do mínimo configurado
- DAP acima de 150 cm (possível erro no CAP)
- Altura acima de 45 m

Em todos os casos, você pode confirmar o registro mesmo com o alerta.

---

## 6. Banco de Espécies

### 6.1 Espécies globais

O Arboris inclui um banco com as 30 espécies mais comuns da Floresta Ombrófila Mista e Floresta Estacional. Disponíveis automaticamente em todos os projetos.

### 6.2 Bancos regionais (Pacotes por Fitofisionomia)

Baixe pacotes de espécies por fitofisionomia em **Hub → Bancos por Fitofisionomia**. Os pacotes são baixados uma vez (sendo necessária conexão com a internet nesta etapa) e ficam disponíveis offline para utilização nos projetos.

Pacotes disponíveis:

- Caatinga nordeste (MG)
- Campos rupestres (MG / BA)
- Cerrado (GO / MT / MS)
- Cerrado (SP / PR / MG)
- Floresta estacional decidual (RS / SC)
- Floresta estacional decidual (PR)
- Floresta estacional decidual (SP / RJ / MG)
- Floresta ombrófila densa amazônica ocidental (AC / RO)
- Floresta ombrófila densa amazônica central (AM)
- Floresta ombrófila densa amazônica meridional (MT)
- Floresta ombrófila densa amazônica oriental (PA / AP)
- Floresta ombrófila densa (BA / ES)
- Floresta ombrófila densa (RS / SC / PR)
- Floresta ombrófila densa sudeste
- Floresta ombrófila mista (PR / SP)
- Floresta ombrófila mista (RS / SC / PR)
- Pampa (RS)
- Portugal continental
- Restinga (SP / PR)
- Restinga sul (RS / SC)

### 6.3 Busca avançada de espécies

Em **Hub → Banco de Espécies**, use os filtros avançados:

- **Origem:** Nativa ou Exótica
- **Grupo Ecológico:** Pioneira, Secundária Inicial, Secundária Tardia, Clímax
- **Status de Conservação (IUCN):** LC, NT, VU, EN, CR, NE — seleção múltipla
- **Escopo:** Banco Global, Projeto ou Pacote instalado

### 6.4 Cadastrar nova espécie

Espécies não disponíveis no banco global podem ser cadastradas manualmente e ficam disponíveis para levantamentos futuros. Em **Banco de Espécies**, toque em **+ Nova Espécie** e preencha: nome científico (obrigatório), nome comum, família, origem, grupo ecológico e status IUCN.

---

## 7. Área de Estudo

Acesse **Hub → Área de Estudo** para configurar a área do projeto:

| Campo | Uso |
|---|---|
| Nome da Área | Identificação no relatório |
| Tamanho (ha) | Obrigatório para Censo Florestal |
| Matrícula do Imóvel | Aparece na seção Caracterização da Área do relatório |
| CAR | Cadastro Ambiental Rural |
| Endereço / Localização | Descrição da localização do imóvel |
| Coordenadas GPS | Ponto central da área para o mapa |
| Fotos da Área | Aparecem no Relatório Fotográfico |

---

## 8. Mapas e GPS

### 8.1 Mapa Interativo (Leaflet)

Acesse **Hub → Visualização → Mapa Interativo**. Funcionalidades:

- Visualização em mapa de satélite com camadas sobrepostas
- Camadas ativáveis: Indivíduos, Parcelas, Pontos PCQM, Polígono da área, Pontos de Interesse
- Toque em um marcador para ver detalhes do indivíduo ou POI
- Polígono da área: defina os vértices diretamente no mapa ou pela tela de Área de Estudo

> 💡 **Dica offline:** A conexão com a internet é necessária para visualização da imagem de satélite. Para uso offline, acesse o Mapa Interativo em local com sinal de internet, abra e aproxime a imagem no local do levantamento para que ela fique gravada em cache.

### 8.2 Coordenadas GPS (tela legado)

**Hub → Coordenadas GPS** exibe a lista de todos os indivíduos com GPS registrado. Toque em qualquer item para abrir a imagem de satélite.

### 8.3 Pontos de Interesse (POIs)

Marque elementos relevantes da área em **Hub → Pontos de Interesse**:

- Tipos disponíveis: Nascente, Córrego, Lago/Represa, Estrada, Edificação, Limite, Outros
- Cada POI tem nome, tipo, descrição, coordenadas GPS e fotos
- POIs aparecem no Mapa Interativo e no Relatório Fotográfico

---

## 9. Resultados, Cálculos e Gráficos

### 9.1 Tela de Resultados e Cálculos *(Plano PRO)*

Acesse **Hub → Análise → Resultados e Cálculos** para visualizar:

- **Resumo:** total de indivíduos, espécies, densidade e área basal por hectare
- **Índices de Diversidade:** Shannon H', Pielou J', Simpson 1-D, Quociente de Mistura
- **Estatística Amostral ACS** (Parcelas Fixas): CV, erro relativo, IC 95%, suficiência amostral
- **Estrutura Vertical CONAMA 392/2007:** estratos Inferior (<5m), Médio (5–12m), Superior (≥12m)
- **Tabela Fitossociológica completa:** DA, DR, FA, FR, DoA, DoR, VC%, VI, VIA por espécie

### 9.2 Gráficos *(Plano PRO)*

Acesse **Hub → Visualização → Gráficos**. Abas disponíveis:

| Aba | Conteúdo |
|---|---|
| 📏 DAP | Distribuição diamétrica por classe + tabela de frequências |
| 🌳 Espécies | Abundância top 8 + pizza proporcional top 5 |
| 📐 Altura | Distribuição de alturas por classe + estratos CONAMA |
| 🌿 Família | Abundância e riqueza por família botânica |
| 📊 Fitossoc. | VI, VIA, DoR, DR, Área Basal por espécie (top 10) |

> 📊 **Exportar Gráficos:** Na aba Fitossoc., toque em **Exportar Gráficos (HTML)** para gerar um arquivo com todos os gráficos em SVG interativo, abrível em qualquer navegador e imprimível como PDF.

---

## 10. Histórico de Edições

O Arboris registra automaticamente todas as criações e edições de indivíduos. Para acessar:

- Abra a **Lista de Indivíduos** do projeto
- Toque no ícone 📋 ao lado de qualquer indivíduo
- Visualize a linha do tempo com data, hora e o que foi alterado

A tela de histórico mostra um snapshot completo do estado do indivíduo em cada evento, incluindo diff visual com campos alterados destacados em vermelho (valor anterior) e verde (novo valor).

> ℹ️ **Observação:** O histórico é gravado a partir da instalação da versão 1.3.0. Indivíduos registrados antes dessa versão não possuem histórico.

---

## 11. Relatórios

### 11.1 Relatório Técnico Word

Acesse **Hub → Análise → Relatório Técnico Word**. O documento gerado inclui:

- Capa com dados do projeto, cliente e responsável técnico
- Sumário automático
- Introdução, Caracterização da Área e Metodologia
- Tabela de coordenadas GPS em DMS
- Resultados com tabela fitossociológica completa
- Índices de diversidade com interpretação
- Distribuição diamétrica e estrutura vertical
- Conclusões e Referências Bibliográficas
- Espaço para assinatura do responsável técnico

### 11.2 Relatório Técnico PDF

Na mesma tela, toque em **📋 Gerar PDF** (não editável). O PDF usa o mesmo template e cores configurados, ideal para:

- Envio a órgãos ambientais (IBAMA, SEMA, IAT, etc.)
- Assinatura digital
- Arquivo formal não editável

### 11.3 Relatório Fotográfico Word/PDF

Acesse **Hub → Análise → Relatório Fotográfico**. Inclui:

- Fotos da Área de Estudo com legendas
- Fotos dos indivíduos agrupadas por árvore
- Fotos dos Pontos de Interesse
- Layout com 2 fotos por linha

> ⚡ **Otimização de memória:** As fotos são comprimidas automaticamente antes de serem inseridas no documento, permitindo gerar relatórios com 50+ fotos mesmo em celulares com pouca RAM.

### 11.4 Templates de Relatório

Personalize a aparência dos relatórios em **Hub → Análise → Relatório Técnico → 🎨 Personalizar Template**:

| Elemento | Opções |
|---|---|
| Logo da empresa | Selecione da galeria (PNG ou JPG) |
| Paleta de cores | 5 paletas predefinidas + personalizada |
| Fonte | Calibri, Arial, Times New Roman, Georgia |
| Tamanho da fonte | 10pt, 11pt, 12pt |
| Template favorito | Marcado com ⭐, carregado automaticamente |

---

## 12. Central de Exportação

Acesse **Hub → Análise → Central de Exportação** para todos os formatos de saída:

| Formato | Conteúdo | Uso |
|---|---|---|
| ZIP Completo | CSV + KML + HTML gráficos + fotos comprimidas + LEIAME.txt | Backup completo do projeto |
| CSV Dados Brutos | Todos os indivíduos com todos os campos | Importar no Excel, R, Python |
| CSV Resultados | Índices fitossociológicos por espécie | Análise estatística |
| SINAFLOR Isoladas | Planilha no formato SINAFLOR para árvores isoladas | Importar no sistema IBAMA |
| SINAFLOR Volume | Planilha no formato SINAFLOR com volume total por espécie | Importar no sistema IBAMA |
| KML | Indivíduos, parcelas, polígono e POIs georreferenciados | Google Earth, QGIS |
| HTML Gráficos | Gráficos interativos em SVG | Relatórios e apresentações |

> 📦 **Backup ZIP:** O ZIP completo inclui todas as fotos comprimidas automaticamente. O arquivo LEIAME.txt dentro do ZIP explica cada arquivo gerado.

---

## 13. Segurança e Privacidade dos Dados

- Todos os dados ficam armazenados localmente no banco SQLite do dispositivo
- Nenhum dado é enviado a servidores externos
- Não há coleta de dados pessoais ou de projeto
- Coletamos apenas analytics anônimos para melhoria do app (sem identificação)
- O backup ZIP pode ser transferido para outro dispositivo ou armazenado na nuvem manualmente

> ⚠️ **Atenção:** Ao desinstalar o aplicativo, todos os projetos e dados são permanentemente excluídos. Sempre faça backup via Central de Exportação antes de desinstalar ou trocar de celular.

---

## 14. Perguntas Frequentes (FAQ)

**O app funciona sem internet?**  
Sim. O Arboris é 100% offline. A internet é necessária apenas para baixar pacotes de espécies, para compras in-app (Plano PRO) e para visualização da imagem de satélite.

**Como transfiro projetos para outro celular?**  
No momento não é possível transferir projetos de um celular para outro. A funcionalidade de importação/compartilhamento de projetos está planejada para versão futura.

**Como transfiro projetos para o computador?**  
Use a **Central de Exportação → ZIP Completo** para fazer backup, ou use as funções de Relatório Fotográfico e Relatório Técnico Word — toque em exportar, selecione e-mail, WhatsApp, salvar no Drive, entre outros.

**Como calculo o DAP a partir do CAP?**  
O app calcula automaticamente. A fórmula é: DAP (cm) = CAP (cm) ÷ π. Para múltiplos fustes, o DAP equivalente é calculado pela soma das áreas basais.

**O que é o erro relativo na Estatística ACS?**  
É a precisão da amostragem por parcelas. Um erro relativo ≤ 10% indica amostragem suficiente para inventários florestais. O app mostra quantas parcelas adicionais são necessárias caso o erro seja maior.

**Posso usar o mesmo banco de espécies em vários projetos?**  
Os pacotes regionais instalados ficam disponíveis em todos os projetos automaticamente. Espécies cadastradas manualmente são específicas de cada projeto (para versões futuras está previsto que espécies cadastradas manualmente fiquem disponíveis para todos os projetos).

**Como ativo o modo escuro?**  
O Arboris segue o tema do Android. Ative em: **Configurações do Android → Tela → Tema Escuro**.

**O relatório Word gerado é editável?**  
Sim. O arquivo .docx pode ser aberto e editado no Microsoft Word, LibreOffice ou Google Docs. O PDF gerado é não editável, recomendado para envio oficial.

---

## 15. Referências Técnicas

### 15.1 Fórmulas utilizadas

| Parâmetro | Fórmula |
|---|---|
| DAP (cm) | CAP ÷ π |
| Área Basal (m²) | π × (DAP/200)² |
| Volume (m³) | AB × Altura × Fator de Forma |
| Volume (mst) | Volume (m³) × Fator de Conversão |
| Densidade Absoluta (DA) | N indivíduos da espécie / Área amostrada (ha) |
| Dominância Absoluta (DoA) | AB total da espécie / Área amostrada (ha) |
| Shannon H' | −Σ (pi × ln pi) |
| Pielou J' | H' / ln(S)  onde S = número de espécies |
| Simpson (1-D) | 1 − Σ (ni(ni−1) / N(N−1)) |

### 15.2 Estratificação Vertical (CONAMA 392/2007)

| Estrato | Altura |
|---|---|
| Inferior | HT < 5 metros |
| Médio | 5 metros ≤ HT < 12 metros |
| Superior | HT ≥ 12 metros |

### 15.3 Status de Conservação IUCN

| Sigla | Significado |
|---|---|
| LC | Least Concern — Menor Preocupação |
| NT | Near Threatened — Quase Ameaçada |
| VU | Vulnerable — Vulnerável |
| EN | Endangered — Em Perigo |
| CR | Critically Endangered — Criticamente em Perigo |
| NE | Not Evaluated — Não Avaliada |

---

*Arboris — App de Levantamento Florestal | Versão 1.3.5 | © 2026 Belenzier Consultoria*

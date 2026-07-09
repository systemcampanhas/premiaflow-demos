# Fabrica de Landing Page Premia Flow

Este guia serve como contexto permanente para criar novas landing pages comerciais no repositório `premiaflow-demos`.

Use esta pasta quando a conversa começar com algo como:

> usar a fabrica de landing page

## Objetivo

Criar landing pages comerciais personalizadas para apresentar o Premia Flow a agencias, CDLs, ACEs, shoppings, varejistas, associacoes comerciais, marcas regionais e outros parceiros.

A pagina deve posicionar o Premia Flow como parceiro operacional, tecnologico e regulatorio para campanhas promocionais digitais, sem competir com o cliente/parceiro apresentado.

## Fluxo esperado

1. Receber o briefing do cliente.
2. Escolher ou confirmar o mockup que sera usado.
3. Criar uma pasta isolada para a landing.
4. Reaproveitar o padrao visual aprovado.
5. Validar localmente.
6. Fazer commit seguro quando autorizado.
7. Publicar apenas via push para o fluxo normal do GitHub Pages.

## Informacoes que preciso receber

Para criar uma nova landing, informar:

- Nome do cliente/parceiro.
- Tipo de organizacao: agencia, shopping, CDL, ACE, varejo, supermercado, associacao, evento, marca regional ou outro.
- Cidade/regiao, se for relevante.
- Contexto comercial da abordagem.
- Objetivo da apresentacao.
- Mockup que deve ser embutido.
- Tom desejado: mais institucional, comercial, consultivo, premium, direto ou leve.
- Contatos de CTA: e-mail, WhatsApp, link de agenda ou placeholder.
- Se pode mencionar apoio regulatorio.
- Se pode usar marcas reais no mockup ou se precisa ser neutro.
- Se ha restricoes de nomes, marcas, logos, textos ou promessas.

## Padrao de pasta

Criar uma pasta por apresentacao:

```text
/nome-da-demo/
  index.html
  assets/
```

Exemplos:

```text
/comunic/
/cdl-nome/
/ace-nome/
/shopping-nome/
/agencia-nome/
```

Usar nomes de pasta em minusculas, sem acentos, sem espacos e com hifens.

## Padrao visual

Base recomendada:

- visual premium, limpo e comercial;
- linguagem B2B;
- primeira dobra forte e objetiva;
- destaque para experiencia mobile;
- mockup dentro de moldura visual de smartphone;
- poucos textos explicativos;
- evitar aparencia de sistema tecnico;
- evitar pagina longa demais;
- responsivo para celular e desktop.
- em secoes de aplicacao, evitar chamadas interrogativas como `Quando pode fazer sentido`; usar linguagem afirmativa, por exemplo `Possibilidades`.

## Estrutura sugerida da landing

1. Hero
   - eyebrow curto;
   - titulo comercial;
   - texto principal;
   - divisao de papeis quando fizer sentido;
   - CTA principal;
   - CTA auxiliar para abrir mockup.

2. Demonstracao
   - moldura de celular;
   - iframe com o mockup escolhido;
   - botao para abrir em nova aba.

3. Como funciona
   - papel do parceiro/cliente;
   - papel do Premia Flow.

4. Onde aplicar
   - usar titulo afirmativo, preferencialmente `Possibilidades`;
   - segmentos ou cenarios de uso.

5. Conversa final
   - CTA por e-mail, WhatsApp ou agenda.

## Papel do cliente/parceiro

Normalmente destacar que o cliente/parceiro lidera:

- estrategia;
- relacionamento com cliente;
- comunicacao;
- criacao;
- midia;
- direcao da campanha;
- conhecimento do mercado local.

Adaptar conforme o tipo de organizacao.

## Papel do Premia Flow

Normalmente destacar que o Premia Flow apoia com:

- experiencia mobile;
- cadastro de participantes;
- cupons;
- numeros da sorte;
- premios instantaneos;
- painel operacional;
- organizacao dos registros;
- rastreabilidade;
- documentacao;
- apoio regulatorio;
- apuracao e acompanhamento.

Quando o pilar regulatorio for importante, usar linguagem responsavel:

> O Premia Flow cuida da estruturacao regulatoria, com apoio de profissionais especializados, documentacao gerada pela plataforma e registros auditaveis.

Evitar promessas absolutas como garantia juridica total.

## Mockups

O mockup embutido deve ser escolhido no briefing.

Exemplos possiveis:

- `../rio-preto-shopping/`
- outra demo existente autorizada;
- uma nova demo neutra criada para a apresentacao.

Regras:

- manter o iframe dentro da moldura de smartphone;
- preservar rolagem interna;
- evitar mockup que confunda o posicionamento comercial;
- confirmar autorizacao quando usar marcas reais ou demos de clientes existentes.

## Requisitos tecnicos

- HTML, CSS e JS simples.
- Sem backend.
- Sem API.
- Sem banco.
- Sem autenticacao.
- Sem dependencias externas obrigatorias.
- Sem deploy manual.
- Hospedagem via GitHub Pages.
- Isolamento por pasta.
- Nao alterar demos existentes sem autorizacao expressa.

## Validacao local

Antes de commit/push, validar:

- `git status`;
- diff limitado ao escopo autorizado;
- `/nome-da-demo/` retorna HTTP 200;
- mockup retorna HTTP 200;
- iframe aponta para o mockup correto;
- botao de nova aba aponta para o mockup correto;
- CTA mailto/WhatsApp/agenda funciona;
- nao ha `localhost` no HTML final;
- desktop ok;
- mobile ok;
- sem overflow horizontal visivel;
- sem dependencias externas obrigatorias;
- sem alteracoes em backend, API, banco, autenticacao ou outras demos fora do escopo.

## Commit

So criar commit quando o usuario autorizar.

Mensagem sugerida:

```text
feat: adiciona landing [nome]
```

ou:

```text
feat: publica landing [nome]
```

Sempre fazer `git add` apenas dos arquivos do escopo.

## URLs publicas

A URL publica segue o padrao:

```text
https://systemcampanhas.github.io/premiaflow-demos/nome-da-demo/
```

Mockups existentes seguem o mesmo padrao:

```text
https://systemcampanhas.github.io/premiaflow-demos/rio-preto-shopping/
```

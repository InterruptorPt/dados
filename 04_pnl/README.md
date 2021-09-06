## Descrição dos dados:

Livros recomendados pelo Plano Nacional de Leitura (2006-2020)

**Fontes:** [PNL 2027](https://pnl2027.gov.pt/np4/livrospnl?cat_livrospnl=catalogo_blx) e [Biblioteca Nacional de Portugal](https://opendata.bnportugal.gov.pt/)

Trabalhámos com várias bases de dados facultadas pelo Plano Nacional de Leitura (PNL): um ficheiro com as recomendações até 2017 (inclusive) e seis ficheiros relativos aos semestres 2018-2020. Nos conjuntos de dados brutos, procedemos a algumas correções manuais na nomenclatura das editoras.

Disponibilizamos os seguintes conjuntos de dados:

- `livros_pre_2017.csv` - dados brutos de livros recomendados pelo PNL entre 2006-2017
- `livros_pos_2017.csv` - dados brutos de livros recomendados pelo PNL após 2017
- `isbn_bnp.csv` - dados consolidados através do cruzamento dos ISBNs fornecidos pelo PNL com os metadados disponibilizados pelo catálogo da Biblioteca Nacional de Portugal

## Esquema dos dados:

### `livros_pre_2017.csv`

- `ISBN` - ISBN do livro
- `Título` - título do livro
- `Autor` - autor do livro
- `Ilustrador` - ilustrador
- `Tradutor` - tradutor do livro
- `Data de edição` - data de edição do livro
- `Editora` - editora do livro
- `Idade02`, `Idade02.1` - Idades de leitura recomendadas
- `Nível de leitura01`, `Nível de leitura02` - Níveis de leitura recomendados
- `Temas01`, `Temas02`, `Temas03` - Temas do livro
- `Formato01`, `Formato02` - Suporte do livro (livro, audiolivro, livros com Cd, etc.)
- `Línguas01`, `Línguas02` - Idioma do livro

### `livros_pos_2017.csv`

- `ISBN:` - ISBN do livro
- `Título:` - título do livro
- `Autor(es)` - autor do livro
- `Ilustrador(es)` - ilustrador
- `Tradutor(es)` - tradutor do livro
- `Editora:` - editora do livro
- `Data de edição:` - data de edição do livro
- `Palavras-chave:` - palavras-chave relativas ao conteúdo do livro
- `Idade:` - Idades de leitura recomendadas
- `Nível de Leitura:` - Níveis de leitura recomendados
- `Tema:` - Temas do livro
- `Formato:` - Suporte do livro (livro, audiolivro, livros com CD, etc.)
- `Língua:` - Idioma do livro
- `Ano PNL` - Ano em que foi integrado no PNL

### `isbn_bnp.csv`

- `ISBN` - ISBN do livro
- `titulo` - título do livro
- `autor` - autor do livro
- `editora` - editora do livro
- `data_publicacao` - data de edição do livro
- `url_BNP` - URL do registo de metadados da BNP

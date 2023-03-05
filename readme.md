# Projeto  de Trabalho de conclusão de curso

Meu_tcc

Composição de Melodias com Aprendizado por
Reforço: Investigando a Teoria da Música como
Ferramenta Para Inferência de Sentimento

O script do colab pode rodar a aplicção original que está no endereço da chamada pela importação "magenta.models.rl_tuner".

Os resultados das melodias em midi geradas podem ser verificadas com os títulos passados como parametro no rlt.generate_music_sequence , e estarão no seu drive do colab.

Os endereços de colab devem ser redirecionados para extração na nuvem do operador.

# Resumo

A composição musical feita com o aprendizado sobre um corpo de músicas, com uso
de RNN, é capaz de gerar linhas melódicas muito convincentes em alguns casos. Contudo,
por estar desprovida de uma estrutura definida, pode acabar gerando melodias sem muito
sentido musical.

Natasha Jaques, Shixiang Gu, Richard E. Turner, Douglas Eck em seu artigo,
propõem uma nova arquitetura, que se utiliza do aprendizado por reforço, para impor
uma estrutura global coerente, otimizando algumas funções de recompensas, enquanto
mantém as propriedades aprendidas com os dados.

Um treinamento RNN feito sobre um grande corpus de música, para prever a
próxima nota em uma melodia, vai ser então refinada em um aprendizado por reforço,
que tem como função de recompensa, a combinação entre e as regras da teoria da música
propostas, e uma cópia da saı́da do treinamento RNN.

Os autores demonstram, que essa arquitetura é capazes de construir melodias mais
consistentes, reduzindo sensivelmente, construções melódicas com aparência aleatória e
resultados sem sentido musical, nessas composições.

As regras da música são implementadas por funções, que estruturam e limitam os
comportamentos das melodias geradas, fornecendo saı́das de recompensas, para o apren-
dizado por reforço. Nesse trabalho vamos interferir nessas funções da teoria da música,
alterar seus parâmetros e hiper parâmetros, seus pesos de saı́da e combinar funções.
Executar testes com o propósito de demonstrar a possibilidade de se incorporar
minimamente, de forma intencional, aspectos de sentido emocional nessas melodias feitas
por máquinas.

Fazer uso desse mecanismo como ferramenta de inserção de sentimentos especı́ficos
nas melodias geradas.

Verificar possı́veis influências de sentimentos nos resultados melódicos, para de-
monstrar a possibilidade, do uso dessas modificações, como ferramentas para esse propósito.

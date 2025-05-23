# English syntax parser with logical programming(Prolog)

## English syntax in formal language

S - Sentence;

P - Pronoun;

N - Noun;

V - Verb;

Adj - Adjective;

Det - Determiner;

Prep - Prepositions;

Pp - Preposition Phrase; 

Vp,Vpp - Verb Phrase; 

Ap,Apa - Adjective Phrase; 

Np,Npp,Npt - Noun Phrase; 


$ S \rightarrow NpVp $

$ Np \rightarrow P | Npp$

$ Npp \rightarrow N | Ap N | DetNpp | NNpt | ApNNpt|DetNppNpt $

$ Npt \rightarrow PpNpt | Npt $

$ Vp \rightarrow V|VNp|VVpp|AdvV|AdvVNp|AdvVVpp$
$ Vpp \rightarrow Pp|PpVpp$

$ Pp \rightarrow Prep|Npp$

$ Ap \rightarrow AdvApa|DetApa|DetAdvApa $

$ Apa \rightarrow Adj|AdjApa$

### File explain

main.pl - main parser

drawer.pl - code for visualization, used pce library 

dict.pl - dictionary with words(facts)

# Analisador lexico
Um analisador léxico, ou scanner, é um programa que implementa um autômato finito, reconhecendo (ou não) strings como símbolos válidos de uma linguagem.

A implementação de um analisador léxico requer uma descrição do autômato que reconhece as sentenças da gramática ou expressão regular de interesse. Com essa descrição, é possível oferecer os seguintes procedimentos auxiliares para o analisador léxico:
* ESTADO-INICIAL, que recebe como argumento a referência para o autômato e retorna o seu estado inicial;
* ESTADO-FINAL, que recebe como argumentos a referência para o autômato e a referência para o estado corrente. O * procedimento retorna true se o estado especificado é elemento do conjunto de estados finais do autômato, ou false caso contrário; e
* PRÓXIMO-ESTADO, que recebe como argumento a referência para o autômato, para o estado corrente e para o símbolo sendo analisado. O procedimento consulta a tabela de transições e retorna o próximo estado do autômato, ou o valor nulo se não houver transição possível.

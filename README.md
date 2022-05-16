## Aulas de Grid


1 - Quando se trata de colunas no grid, a primeira coluna é a coluna de esquerda para direita. e é sempre coloca a sintaxe no plural. "grid-template-columns".

2 - Unidade de medida: fr ou seja o fracional.
    grid-template-columns: 1fr 1fr fr1;

    1fr = 1 fracional de largura. - se tiver conteúdo dentro da coluna, ocupa todo o espaço disponível.


3 - minmax - será defindo tamanho minino e o tamanho maximo.
    grid-template-columns: minmax(100px, 1fr) 1fr;

    minmax(100px, 1fr) = 100px = 100px de largura mínima e 1fr = 1 fracional de largura.

4 - repeat - será repetindo o conteúdo da coluna.
    grid-template-columns: repeat(2, 1fr);

    repeat(2, 1fr) = 2 vezes 1 fracional de largura.

    <!-- posso usar como responsivo - sem mexer muito em midia query -->
    grid-template-columns: repeat(auto-fit, minmax(100px, auto)); 1fr;

    *Ele preenche quando tiver conteudo, quando não tiver conteudo, preenche com o tamanho mínimo.

5 - auto-fill - será preencher o espaço disponível.
    grid-template-columns: auto-fill;

    auto-fill = preencher o espaço disponível.

    *Ele prennche o espaço disponível ou seja a coluna que tiver vazia, com o tamanho pré definido.
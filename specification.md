# Simulação Semáforo - IA

## Agentes

### Semáforo

Este agente atuará no controle do sentido que o veículo tomará ao trafegar pelas vias. O sentido será gerado randomicamente por outro agente. Para saber quando deve liberar ou não o tráfego, o semáforo ferá requisições para seu agente superior, o cruzamento, e este retornará uma resposta permitindo ou não a liberação da via em determinado sentido.

### Cruzamento

O agente cruzamento atuará no controle dos semáforos. Assim como o agente citado anteriormente, o cruzamento fará requisições ao seu superior, o bairro, para saber o tempo que um determinado semáforo poderá ficar aberto. Dependendo do tráfego no momento, o cruzamento, com a devida permissão, permitirá que um semárofo abra.

### Bairro

O agente bairro controlará todos os cruzamentos de uma determinada região. Sua função é orquestrar os cruzamentos para que o tráfego flua sem congestionamentos. Constantemente enviará para o seu agente superior informações sobre sua região para que este possa tomar as melhores decisões.

### Cidade

Já o agente cidade atuará no controle de todos os bairros. Com informações dos agentes bairro, poderá desafogar uma região e assim equilibrar o tráfego dos veículos.

O fluxo da informação entre os agentes sempre será de uma requisição para seu superior e uma resposta para seu subordinado.

Cada agente só saberá de suas atividades, ou seja, um semáforo A só terá controle de si mesmo, sem saber o estado em que o semáforo B está do mesmo jeito que um bairro C só orquestrará o tráfego de sua própria região, sem saber como está o bairro D.
# Seu plantão termina. A operação continua.

**Um guia prático para escrever procedimentos de TI que outra pessoa consegue executar.**

Para equipes de suporte, infraestrutura e sistemas.

## Sumário

1. [Escolha uma rotina que merece um procedimento](#escolha-uma-rotina-que-merece-um-procedimento)
2. [Escreva para quem vai executar](#escreva-para-quem-vai-executar)
3. [Veja um procedimento em ação](#veja-um-procedimento-em-ação)
4. [Teste antes de publicar](#teste-antes-de-publicar)
5. [Copie o modelo para sua próxima rotina](#copie-o-modelo-para-sua-próxima-rotina)

## Escolha uma rotina que merece um procedimento

Imagine que o plantão começa com um chamado: a fila de impressão parou. A pessoa que costuma resolver está de folga. O histórico mostra que alguém “ajustou a fila” no último incidente. Ninguém sabe qual fila, como o ajuste foi feito ou como comprovar que a impressão voltou.

Um bom procedimento responde a três perguntas de quem recebeu o chamado: **o que preciso verificar, até onde posso agir e como sei que terminei?** Escolha uma rotina real e escreva para uma situação específica, com um começo e um fim observáveis.

### Escolha seu primeiro caso

- **Frequência:** a tarefa aparece com regularidade ou interrompe o trabalho quando falha.
- **Dependência:** poucas pessoas sabem onde verificar ou com quem falar.
- **Critério de conclusão:** existe um resultado que outra pessoa consegue observar e confirmar.

Comece pequeno. “Diagnosticar a fila de impressão compartilhada” cabe em um procedimento. “Resolver todos os problemas de impressão” mistura sintomas, equipamentos e permissões. Cada cenário adicional aumenta a chance de alguém seguir uma etapa errada.

> **Exercício de cinco minutos.** Escreva o gatilho e o resultado em uma frase. Exemplo: “Quando duas estações não conseguirem imprimir na mesma fila, confirmar se a falha é compartilhada e registrar as evidências no chamado.”

## Escreva para quem vai executar

O procedimento começa antes do primeiro clique. Diga quais acessos a pessoa precisa, onde encontrar o equipamento ou sistema e quem pode autorizar ações que afetem outros usuários.

### Dê a cada passo uma saída visível

- **Ação:** descreva o que fazer e em qual interface ou local.
- **Resultado esperado:** indique o sinal que confirma a etapa.
- **Decisão:** diga o que fazer se o resultado for diferente do esperado.

**Exemplo:** “Envie uma página de teste sem dados pessoais pela mesma fila. Confirme se ela aparece na fila e se sai na impressora. Se o trabalho ficar retido, registre o estado e o horário antes de escalar.”

Use verbos específicos. “Verifique a impressora” permite interpretações demais. “Confirme que a impressora está ligada e anote o aviso exibido no painel” permite reproduzir e comparar o diagnóstico.

### Marque o limite de atuação

Identifique ações de leitura e ações que mudam o ambiente. Se a intervenção autorizada falhar, diga quem recebe o escalonamento e o que precisa chegar junto ao chamado. Registre o passo de retorno ao estado anterior quando houver alteração reversível.

> **Regra prática.** Um print ajuda quando mostra um campo difícil de encontrar. Acrescente o nome do caminho ou do menu em texto para que o procedimento continue útil quando a tela mudar.

## Veja um procedimento em ação

### Exemplo fictício: fila de impressão compartilhada

**Gatilho.** Duas estações relatam falha na mesma fila.  
**Objetivo.** Separar falha local de falha compartilhada e produzir evidências para continuidade.  
**Pré-requisitos.** Chamado aberto, acesso à fila e página de teste sem informações pessoais.

1. **Identifique a fila.** Confirme o nome exibido nas duas estações e registre o setor, o horário e a mensagem. Se os nomes forem diferentes, trate cada fila como um caso separado.
2. **Confirme o sintoma.** Envie uma página de teste de uma estação autorizada. Observe se o trabalho chega à fila e anote se imprime, fica retido ou desaparece.
3. **Verifique o equipamento.** Observe energia, papel e aviso no visor. Resolva apenas as condições locais previstas para seu perfil de acesso.
4. **Repita a verificação.** Faça um novo teste com o mesmo tipo de documento. Se a impressão voltar, confirme a saída física e peça retorno a uma das estações afetadas.
5. **Feche ou escale.** Se o problema continuar em mais de uma estação, encaminhe ao responsável pela fila com nome, horário, mensagem, teste feito e impacto. Alterações no servidor e limpeza da fila compartilhada seguem a autorização da equipe responsável.

> **Evidência de conclusão.** Página de teste impressa e funcionamento confirmado por uma estação afetada. Se a falha continuar, registre o encaminhamento e mantenha o chamado aberto.

## Teste antes de publicar

Entregue o rascunho a alguém que conhece o ambiente, mas nunca executou aquela rotina. Dê o cenário e deixe a pessoa trabalhar com o texto. Observe o que ela precisa perguntar, onde hesita e que verificações faz por iniciativa própria.

### O que observar no ensaio

- A pessoa encontrou o alvo correto e tinha os acessos necessários?
- Conseguiu identificar quando continuar, parar ou escalar?
- Chegou à mesma conclusão que você usando evidências observáveis?
- Outra pessoa conseguiria retomar o chamado com o registro deixado?

Se o teste exigir ajuda verbal, transforme a orientação em uma frase no ponto onde surgiu a dúvida. Repita o passo alterado com outra pessoa ou peça que a mesma pessoa descreva o fluxo a partir do roteiro.

### Dê um dono e um motivo para revisar

Publique o procedimento onde a equipe já trabalha e vincule-o ao tipo de chamado correspondente. Registre responsável, versão e data da última validação. Revise quando a interface mudar, o fluxo de aprovação for alterado ou alguém precisar de uma instrução que não está no texto.

> **Teste de manutenção.** Abra o último chamado resolvido com o procedimento e veja se a evidência registrada confirma o resultado definido no documento.

## Copie o modelo para sua próxima rotina

Use uma frase por campo para montar o rascunho. Expanda apenas as etapas em que uma decisão ou uma dependência precisa ficar explícita.

- **Título:** verbo de ação e alvo da rotina.
- **Gatilho e escopo:** quando usar e qual situação encaminhar por outro fluxo.
- **Responsável e pré-requisitos:** perfil de acesso, materiais e dependências.
- **Passos:** ação, resultado esperado e alternativa se falhar.
- **Ponto de parada:** ação que exige autorização e destinatário do escalonamento.
- **Conclusão:** evidência mínima de sucesso e onde registrá-la.
- **Manutenção:** dono, versão, data de validação e condição de revisão.

### Antes de publicar

- [ ] O cenário é específico e alguém consegue reconhecer o gatilho.
- [ ] Os passos têm resultado esperado e limites de atuação claros.
- [ ] O encerramento exige uma evidência que outra pessoa consegue conferir.
- [ ] Um colega executou a rotina usando o texto.
- [ ] A versão publicada tem responsável e data da última validação.

**Pegue um chamado recorrente desta semana. Escreva o gatilho, defina a evidência de conclusão e entregue o primeiro rascunho a um colega para testar.**

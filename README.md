# micro-exercicios

Uma lista exercícios pequenos e com desafios variados.  
O propósito desse repositório é ser utilizado por quem ta sem ideias, pretende aprender algo novo ou quer obter experiência de situações possivelmente reais.  
Muitos dos exercícios tem como objetivo fazer que ativamente erros sejam cometidos, mitigados, entendidos e resolvidos.  
Abrace os erros, aprenda com eles.  


## Ferramental

### Ambientes Virtuais

1. **Problema:** Crie um ambiente virtual para a linguagem de programação da sua escolha.  
**Situação:** Você vai iniciar um projeto e precisa isolar os pacotes que vai instalar, dos pacotes instalados globalmente.

1. **Problema:** Crie dois ambientes virtuais, instale em um deles uma versão de um pacote, e instale no outro uma outra versão.  
**Situação:** Você está lidando com mais de um projeto, e eles usam o mesmo pacote, porém em versões diferentes.

1. **Problema:** Crie dois ambientes virtuais. Instale, em cada uma delas, diferentes versões da linguagem de programação que você escolheu.  
**Situação:** Você está trabalhando em mais de um projeto, e cada projeto usa uma versão diferente da mesma linguagem.


### Git

1. **Problema:** Crie um repositório online e clone para o seu local.  
Utilize diferentes plataformas para criar o repositório, como Github, Gitlab e Bitbucket.  
**Situação:** Você precisa criar um projeto novo.

1. **Problema:** Crie localmente uma branch, adicione um commit e dê push para a branch de mesmo nome no repositório remoto.  
**Situação:** Você fez uma modificação e precisa que ela fique disponível para outras pessoas do seu trabalho.

1. **Problema:** Adicione um novo commit numa branch que esteja atualizada remotamente e não dê push.
Então crie uma branch nova baseada na branch remota(que não possui o commit que a local tem).  
**Situação:** Você está trabalhando em um problema, mas precisa pausar e ir trabalhar em outro, porém ambos tem origem na mesma branch.

1. **Problema:** Adicione um commit localmente e dê push da sua branch local para a branch de nome diferente no repositório.
Ex: se sua branch local se chama master, então envie para a branch algumacoisa .  
**Situação:** Você começou a trabalhar numa branch local, e durante a resolução descobriu que vai precisar enviar as alterações para uma branch remota específica.

1. **Problema:** Adicione um novo servidor remoto diferente do origin no seu git local, e dê um push para ele.  
Ex: vamos supor que você criou dois repositórios, um no github e um no gitlab. Você clonou o do github para seu local.  
Então o seu origin vai estar apontando pro repositório no github.  
Crie localmente um outro remoto localmente com um nome diferente de origin e aponte ele para o gitlab.  
**Situação** Num mesmo projeto você vai utilizar mais de uma plataforma.



## Backend

### Servidores

1. **Problema:** Escreva e rode um servidor http utilizando a linguagem/aplicação/framework de sua escolha.  
O retorno dela pode ser um simples hello world.  
**Situação:** Você esta iniciando um projeto de um novo servidor http.

1. **Problema:** Tente rodar, ao mesmo tempo, duas instâncias do servidor na mesma porta.  
Tente entender o motivo de não funcionar.

1. **Problema:** Rode, ao mesmo tempo, o mesmo servidor em portas diferentes.  
Ex: rode um na 5000 e outro na 3000.  
**Situação:** Você precisa que duas instâncias do servidor sejam executadas ao mesmo tempo.

1. **Problema:** Rode, um de cada vez, o servidor num dos seguintes hosts: 0.0.0.0, localhost e 127.0.0.1.  
Pesquise sobre o assunto host. Depois teste e experimente quem na rede pode acessar o servidor.  
Isso é importante para configurar corretamente o servidor e evitar que seja acessado por alguém indevidamente.  
**Dica:** Se seu computador e celular estiverem no mesmo wifi, tente acessar o servidor do seu computador pelo celular.  
**Situação:** Você esta configurando um servidor para que ele funcione corretamente.

### Cache

1. **Problema:** Escreva um servidor http utilizando a linguagem/aplicação/framework de sua escolha.  
Crie uma rota, com método GET, que receba um número pelo path/caminho e retorne o dobro dele.  
Configure para que essa rota seja cacheada.  
Para o cache utilize uma ferramenta como o redis ou memcached.  
**Dica:** Para ficar fácil de visualizar a diferença entre o com e sem o cache, configure um sleep nessa rota.  
**Situação:** Você quer otimizar o tempo da requisição e utilização dos recursos do servidor utilizando cache.

1. **Problema:** Em um servidor http que possui uma rota com cache, configure o 'time to live'/expire do cache.  
**Dica:** Para fins de desenvolvimento, coloque para o cache expirar com um tempo relativamente curto, como 1 minuto.  
**Situação:** Você quer que cache expire para forçar atualização ou para evitar bugs.

1. **Problema:** Um servidor http possui uma rota com metódos POST e GET.  
O servidor guarda numa variável o valor de um número que inicia em 0.  
No caso de POST, deve se passar um número que substitui o valor da variável.  
No caso do GET, retorne o dobro do valor na variável.  
O método GET da rota possui cache.  
Sempre que a rota receber um POST, você deve revogar/expirar/deletar o cache do metódo GET da rota.  
**Situação:** Você tem que expirar o cache após fazer alguma alteração. Para que não retorne um valor desatualizado.


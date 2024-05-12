**Criando um Pipeline de Deploy de uma Aplicação Utilizando Gitlab, Docker e Kubernetes**

Este artigo mostra como criar um pipeline de deploy de uma aplicação utilizando Gitlab, Docker e Kubernetes. Este pipeline será usado para implantar uma aplicação simples de hello world em um cluster Kubernetes.

## **Requisitos**

Para seguir este tutorial, você precisará dos seguintes requisitos:

- Um cluster Kubernetes

- Um servidor Gitlab

- Uma conta de usuário no Gitlab

- Uma chave SSH pública que seja adicionada ao seu perfil de usuário no Gitlab

- Uma imagem Docker da aplicação que você deseja implantar

  

#### **Etapa 1: Criar um projeto no Gitlab**

O primeiro passo é criar um projeto no Gitlab. Para isso, acesse o site do Gitlab e faça login na sua conta. Em seguida, clique no botão **Novo projeto** e preencha os campos obrigatórios.



#### **Etapa 2: Criar uma imagem Docker da sua aplicação**

O próximo passo é criar uma imagem Docker da sua aplicação. Para isso, você pode usar um comando como o seguinte:

```plaintext
docker build -t myapp .
```

Este comando criará uma imagem Docker chamada `myapp` baseada no código-fonte da sua aplicação.



#### **Etapa 3: Criar uma pipeline de deploy no Gitlab**

O terceiro passo é criar uma pipeline de deploy no Gitlab. Para isso, acesse o seu projeto no Gitlab e clique no botão **Pipelines**. Em seguida, clique no botão **Novo** e selecione o tipo de pipeline `Kubernetes`.

Na página de configuração da pipeline, você precisará fornecer as seguintes informações:

- O nome do seu cluster Kubernetes
- A chave SSH pública que você adicionou ao seu perfil de usuário no Gitlab
- O nome da sua imagem Docker
- O nome do seu pod
- O número de réplicas

Depois de preencher as informações necessárias, clique no botão **Salvar** para criar a sua pipeline de deploy.

**Etapa 4: Testar a sua pipeline de deploy**

Agora que você criou a sua pipeline de deploy, é hora de testá-la. Para isso, faça um commit e push para o seu projeto no Gitlab.

Depois de fazer o commit e push, a sua pipeline de deploy será executada automaticamente. Você pode acompanhar o progresso da sua pipeline na página de pipelines do seu projeto no Gitlab.

Se a sua pipeline de deploy for executada com sucesso, você verá uma mensagem de sucesso na página de pipelines.

**Conclusão**

Neste artigo, você aprendeu a criar um pipeline de deploy de uma aplicação utilizando Gitlab, Docker e Kubernetes. Este pipeline pode ser usado para implantar qualquer aplicação em um cluster Kubernetes.



## Criando-um-Pipeline-de-Deploy-com-GitLab-e-Kubernetes

 Criado um pipeline de deploy de uma aplicação com cenários de produção de imagens com Docker e criação dos deployments em um cluster kubernetes em nuvem utilizando o GCP.


![download](https://user-images.githubusercontent.com/87867234/194542240-feb5e21e-3d0a-4691-865c-2c9f228ed248.jpg)

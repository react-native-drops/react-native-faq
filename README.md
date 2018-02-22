# React Native F.A.Q

Este é um documento colaborativo. Qualquer um pode contribuir mesmo que não faça parte da organização (via fork).
Antes de contribuir, verifique as issues. Escolha uma issue e mãos à obra. 
Caso não encontre uma issue para sua contribuição, crie sua issue.

Junte-se a nós no Telegram também:

React Native Drops - https://t.me/reactnativedrops


## Expo (https://expo.io/)

### O que é Expo?

Expo (antigo Exponent) é um conjunto de ferramentas e bibliotecas open source (toolchain) construído em cima do React Native.
Seu objetivo principal é auxiliar na construção de aplicações nativas em iOS e Android usando Javascript e React.
Além das ferramentas e bibliotecas, uma série de serviços foram incorporados/integrados ao Expo - push notifications e publicação nas lojas de apps são um exemplo.

### Quando não usar Expo?

Expo não está pronto mas está em constante evolução. Algumas bibliotecas e APIs ainda não são suportadas como por exemplo, suporte a bluetooth. Nesse caso, você terá que fazer um 'eject' e usar React Native puro.  Por isso, é importante levantar estes requisitos não-funcionais antes decidir usar Expo.

Outra deficiência do Expo, pelo menos por enquanto, é que ele não suporta código rodando em background. Ou seja, se você precisa fazer tracking de geolocalização em background, tocar aúdio em backeground, gerenciar push notifications em background, esqueça o Expo. Mas é bom saber que essa feature está em desenvolvimento e será liberada em breve.

Outra coisa, se você precisa muito que seu binário de seu app seja muito pequeno, atenção. Qualquer app feito com Expo terá 25mb (iOS) ou 20mb (Android). Por que isso? Bom, Expo inclui uma série de bibliotecas no Expo SDK. E mesmo que você use apenas uma delas (notificações, por exemplo), você carregará todo o restante das bibliotecas no pacote final. A boa notícia que isso já está sendo tratado e em breve seus apps serão mais "magros".

E por último, se você quiser usar um serviço especfico de push notification, OneSignal por exemplo, e não o serviço de Push Notification do Expo, você vai precisar usar ExpoKit ou React Native puro.




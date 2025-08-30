# Estudos sobre React Native - AGES 2025/2  

Este repositório contém meus estudos sobre **React Native** e conceitos relacionados a desenvolvimento **nativo e híbrido** para a disciplina de **AGES 2025/2**.  

---

# Inicio 

Sobre ReactNative:  
* É um Framework JavaScript  
* Permite criar aplicações Mobile  
* É um projeto Open Source mantido pelo Facebook  

Alguns pontos sobre ReactNative:  
* ReactNative =! React  
  - React é uma biblioteca JavaScript para construir interfaces Web.  
  - ReactNative utiliza o React para renderizar aplicações Android e iOS  
* Utiliza Component Mobile ao invés de HTML como o React.  
* Permite criar apps para Android e iOS com a mesma base de código.  

---

# Desenvolvimento Nativo e Híbrido 

## Desenvolvimento Nativo
* Utiliza linguagens oficiais de cada sistema operacional.  
* Android: Java ou Kotlin.  
* iOS: Swift ou Objective-C.  

Pontos importantes:  
* Melhor desempenho, pois o código é executado diretamente no sistema.  
* Acesso total aos recursos do dispositivo (câmera, GPS, sensores etc).  
* Experiência de usuário mais fluida e integrada.  
* Exige desenvolvimento separado para cada plataforma, aumentando tempo e custo.  

## Desenvolvimento Híbrido
* Utiliza um único código para múltiplas plataformas (Android e iOS).  
* Frameworks comuns: React Native, Flutter, Ionic.  

Pontos importantes:  
* Reduz custos e tempo de desenvolvimento, já que parte do código é compartilhado.  
* Permite manutenção mais simples.  
* Pode ter limitações de performance em comparação ao nativo.  
* Pode necessitar de código adicional para acessar recursos específicos do dispositivo.  

---

# Node.js e NPM no React Native

## Node.js
* É um **ambiente de execução JavaScript** fora do navegador.  
* Permite executar ferramentas de desenvolvimento do React Native.  
* Serve como base para o **React Native CLI** e scripts do projeto.  

## NPM
* É o **gerenciador de pacotes do Node.js**.  
* Permite instalar bibliotecas e dependências do projeto, como React e React Native.  
* Facilita atualizar, remover ou gerenciar versões de pacotes, mantendo o projeto organizado.  

Resumo:  
* **Node**: executa JavaScript fora do navegador e permite rodar ferramentas do React Native.  
* **NPM**: gerencia todas as bibliotecas que seu app precisa.  

---

# Expo

O **Expo** é uma plataforma que facilita o desenvolvimento de aplicativos em **React Native**, fornecendo ferramentas que agilizam o processo de criação, teste e publicação.  

Principais vantagens do Expo:  
* 🚀 Rápida inicialização de projetos React Native.  
* 📱 Testes simples no celular via **Expo Go**.  
* 🔧 Conjunto de APIs prontas para uso (câmera, notificações, sensores, etc).  
* 🌍 Publicação facilitada para as lojas de aplicativos.  

### Expo Go
O **Expo Go** é o aplicativo que permite executar projetos Expo no celular sem precisar compilar o código.  
Basta escanear o **QR Code** gerado pelo comando `npx expo start`.  

Links para download:  
* [Expo Go para Android (Google Play)](https://play.google.com/store/apps/details?id=host.exp.exponent)  
* [Expo Go para iOS (App Store)](https://apps.apple.com/app/expo-go/id982107779)  

---

# Criando um projeto Expo com Blank (TypeScript)

Para iniciar um projeto **React Native** usando **Expo** com template **Blank (TypeScript)**:

1. Abra o terminal na pasta onde deseja criar o projeto.  
2. Rode o comando:

```bash
npx create-expo-app SEU_NOME_AQUI -t blank-typescript

---

# Principais comandos do Expo

Depois de criar um projeto Expo, você vai usar alguns comandos no terminal para rodar, testar e publicar seu app.  

## Comandos mais usados:

* `npm start` ou `npx expo start`  
  - Inicia o **Metro Bundler** e abre o **Expo DevTools** no navegador.  
  - Mostra um **QR Code** para testar o app no celular com **Expo Go**.  

* `npm run android` ou `npx expo run:android`  
  - Roda o app diretamente em um **emulador Android** ou dispositivo conectado.  

* `npm run ios` ou `npx expo run:ios`  
  - Roda o app diretamente em um **emulador iOS** (Mac necessário) ou dispositivo conectado.  

* `npm run web` ou `npx expo start --web`  
  - Abre o app no navegador como **web app**, útil para testes rápidos.  

* `npx expo publish`  
  - Publica o app para teste via **Expo Go** sem gerar uma build nativa.  

* `npx expo build:android` ou `npx expo build:ios`  
  - Cria versões **APK** (Android) ou **IPA** (iOS) prontas para envio às lojas.  

> Dica: o comando mais usado durante o desenvolvimento é **`npm start`** ou **`npx expo start`**, pois permite ver as alterações em tempo real no celular.

## Automatização mobile - Setup Appium - Tutorial

### Pré-requisitos para utilização do Appium:

1- NodeJs - https://nodejs.org/pt/download

2- JDK 11 Java - https://www.oracle.com/java/technologies/javase/jdk11-archive-downloads.html

### Setup appium:

1- Install Appium 2.0

    npm i -g appium

2- Verificar se foi instalado corretamente:

    appium -v

3- Install Appium UIAutomator2

    appium driver install uiautomator2

4- Install Appium Doctor

    npm install -g appium-doctor

depois:

    appium-doctor --version

5- Appium doctor para verificar se foi instalado corretamente:

    appium-doctor --android

6- Install latest Android Studio via exe file - https://developer.android.com/studio

7- Install Appium Inspector - github.com/appium/appium-inspector/releases




8- Env variable setup

  - Abra o Android Studio

  - Na tela inicial clique o item Configure e depois no item SDK Manager

  - Copie o caminho apresentado no campo Android SDK Location

  -  Vá até as Variáveis de Ambiente no Windows e:

      - Adicione a seguinte variável com o respectivo valor e clique em OK

         a. Nome da variável: `ANDROID_HOME`

         b. Valor da variável: Diretório presente no campo ***Android SDK Location***

      - Selecione a variável `PATH` e clique em Editar...
    
      - Clique no botão Novo e adicione o seguinte valor de variável
         a.  `o %ANDROID_HOME%\tools`

      - Clique novamente no botão Novo e adicione o seguinte valor de variável

         a. `%ANDROID_HOME%\tools\bin`

      - Clique novamente no botão Novo e adicione o seguinte valor de variável

         a. `%ANDROID_HOME%\platform-tools`



9- Verificar o setup: adb devices ou adb

10- Instalar um novo dispositivo: https://developer.android.com/studio/run/managing-avds?hl=pt-br

11- INSTALAR OS APLICATIVOS NO EMULADOR: https://drive.google.com/drive/folders/1soPlNjkL5MIgvbXNMmuusbbxZmVNVPfG




### Capabilities:

{

"appium:platformName": "Android",

"appium:platformVersion": "13.0",

"appium:automationName": "UIAutomator2",

"appium:deviceName": "emulator-5554",

"appium:appPackage": "io.appium.android.apis",

"appium:appActivity": ".ApiDemos"

}




### Para iniciar o ambiente:

1- emulador(Por meio do Android studio)

2- appium (Por meio da linha de comando)

3- appium inspector

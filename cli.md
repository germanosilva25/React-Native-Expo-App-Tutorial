To check if a user is logged in to Expo via the CLI, you can use the following command:

```bash
expo whoami
```

This command will display the currently logged-in user's information. If no user is logged in, it will prompt that you are not logged in.

### If You Need to Log In
If no user is logged in, you can log in using:

```bash
expo login
```

To change the account logged into the Expo CLI, you can follow these steps:

1. **Log out of the current account**:
   Run the following command to log out of the current user:
   ```bash
   expo logout
   ```

2. **Log in with a different account**:
   After logging out, you can log in with a different account:
   ```bash
   expo login
   ```


   Esse erro ocorre porque o Expo está tentando rodar o aplicativo no modo **development build**, mas você ainda não criou e instalou um build de desenvolvimento no seu dispositivo.  

### 🔧 **Como Resolver?**  

#### 1️⃣ **Criar um Development Build**
Execute o seguinte comando para gerar um build de desenvolvimento:  
**Esse comando cria a pasta /android**
```sh
npx expo run:android
```
Isso criará e instalará o app no seu emulador/dispositivo.

Se você estiver no iOS, use:
```sh
npx expo run:ios
```
> 📌 **Observação**: Se você estiver usando o **Expo Go**, ele **não** suporta pacotes com bibliotecas nativas personalizadas. Você precisa usar um build de desenvolvimento.

#### 2️⃣ **Instalar o Build no Celular**
Se o build foi gerado na **nuvem** (EAS Build), instale-o manualmente no celular:  
```sh
npx expo install:android
```
Ou para iOS:
```sh
npx expo install:ios
```

#### 3️⃣ **Tentar Novamente**
Após instalar o build de desenvolvimento, rode novamente:
```sh
npx expo start
```

Se ainda tiver problemas, me avise! 🚀

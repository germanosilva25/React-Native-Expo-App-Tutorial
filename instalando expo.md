Para instalar o **Expo** no Windows e iniciar projetos **React Native** de forma fácil, siga os passos abaixo:  

---

### **1️⃣ Pré-requisitos**
Antes de instalar o Expo, você precisa ter:  

✔️ **Node.js** instalado  
✔️ **npm** (vem junto com o Node.js) ou **Yarn**  
✔️ **Git** (opcional, mas recomendado)  

Se você ainda não tem o **Node.js**, instale com o [nvm-windows](https://github.com/coreybutler/nvm-windows) ou baixe o instalador em:  
🔗 [https://nodejs.org](https://nodejs.org)  

Depois, verifique se o Node.js e o npm estão instalados corretamente:  
```powershell
node -v
npm -v
```

Se quiser usar o **Yarn** (alternativa ao npm), instale com:  
```powershell
npm install --global yarn
```

---

### **2️⃣ Instalando o Expo CLI**
Agora, instale a CLI do Expo globalmente com o npm ou Yarn:

#### **Com npm:**
```powershell
npm install --global expo-cli
```
#### **Com Yarn:**
```powershell
yarn global add expo-cli
```

Verifique se a instalação foi bem-sucedida:
```powershell
expo --version
```

---

### **3️⃣ Criando um novo projeto Expo**
Agora, crie um novo projeto Expo com:

```powershell
expo init meu-projeto
```
Isso abrirá um assistente onde você pode escolher o template do projeto (por exemplo, **"Blank"** para um projeto básico).

Depois de criar o projeto, entre na pasta:
```powershell
cd meu-projeto
```

E inicie o servidor de desenvolvimento do Expo:
```powershell
expo start
```

Isso abrirá o **Expo DevTools** no navegador e exibirá um QR code para rodar o app no celular.

---

### **4️⃣ Rodando o app no celular**
Para testar seu app no celular:  
📱 **Android**: Baixe o **Expo Go** na Play Store  
📱 **iPhone**: Baixe o **Expo Go** na App Store  

Escaneie o QR code gerado no terminal ou no Expo DevTools para rodar o app no seu celular.

---

### **5️⃣ Rodando em emuladores**
Se quiser rodar o Expo no **Android Emulator** ou **iOS Simulator**:  

#### **Android Emulator (Windows)**
1. Instale o **Android Studio**:  
   🔗 [https://developer.android.com/studio](https://developer.android.com/studio)
2. Abra o Android Studio e configure um **dispositivo virtual**.
3. Ative a opção de **depuração USB** e inicie o emulador.
4. No terminal, execute:
   ```powershell
   expo start --android
   ```
   O Expo abrirá no emulador.

⚠️ O **iOS Simulator** só funciona no macOS.

---

### **🔥 Conclusão**
Agora você tem o **Expo instalado no Windows** e pode criar e testar apps **React Native** facilmente. 🚀  

Se tiver dúvidas ou erros durante a instalação, me avise! 😊
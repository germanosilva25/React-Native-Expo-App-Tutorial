## **Guia Completo: Instalação do Node.js e NVM e Como Eles Funcionam Juntos**

### **1. O Que São Node.js e NVM?**
- **Node.js** é um ambiente de execução JavaScript que permite rodar código JavaScript no servidor, sem a necessidade de um navegador.
- **NVM (Node Version Manager)** é um gerenciador de versões do Node.js que facilita a instalação, atualização e troca entre diferentes versões.

Com o **NVM**, você pode instalar várias versões do Node.js e alternar entre elas conforme necessário.

---

## **2. Instalando o NVM e o Node.js no Windows**
O Windows não tem suporte oficial para o NVM original, mas existe uma alternativa chamada **nvm-windows**.

### **Passo 1: Baixar e Instalar o NVM-Windows**
1. Acesse o repositório oficial:  
   👉 [https://github.com/coreybutler/nvm-windows/releases](https://github.com/coreybutler/nvm-windows/releases)
2. Baixe o arquivo **nvm-setup.exe**.
3. Execute o instalador e siga os passos:
   - Escolha a pasta onde o **NVM** será instalado (padrão: `C:\Program Files\nvm`).
   - O instalador também configura o caminho para o **Node.js** automaticamente.
4. Após a instalação, reinicie o computador para garantir que as variáveis de ambiente foram aplicadas corretamente.

### **Passo 2: Verificar a Instalação**
Abra o **Prompt de Comando (CMD)** ou **PowerShell** e digite:
```sh
nvm version
```
Se estiver instalado corretamente, ele retornará a versão do NVM.

### **Passo 3: Instalar o Node.js Usando o NVM**
Agora você pode instalar qualquer versão do **Node.js** com um simples comando:

1. Liste as versões disponíveis:
   ```sh
   nvm list available
   ```
2. Instale a versão desejada (por exemplo, a mais recente LTS):
   ```sh
   nvm install 18
   ```
3. Ative a versão instalada:
   ```sh
   nvm use 18
   ```
4. Verifique a versão ativa:
   ```sh
   node -v
   ```
   Se o comando retornar algo como `v18.x.x`, significa que a instalação foi bem-sucedida.

---

## **3. Instalando o NVM e o Node.js no Linux/macOS**
No Linux/macOS, usamos o **NVM oficial**.

### **Passo 1: Instalar o NVM**
Abra o **Terminal** e execute:
```sh
curl -fsSL https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.4/install.sh | bash
```
Após a instalação, adicione o NVM ao seu terminal:

```sh
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
```
Caso esteja usando **Zsh** (em vez de Bash), adicione isso ao `~/.zshrc`.

### **Passo 2: Verificar a Instalação**
Reinicie o terminal e digite:
```sh
nvm --version
```
Se tudo estiver correto, ele mostrará a versão instalada do NVM.

### **Passo 3: Instalar e Usar o Node.js**
1. Liste as versões disponíveis:
   ```sh
   nvm ls-remote
   ```
2. Instale a versão desejada:
   ```sh
   nvm install 18
   ```
3. Defina essa versão como padrão:
   ```sh
   nvm alias default 18
   ```
4. Verifique a instalação:
   ```sh
   node -v
   ```
   Se retornar algo como `v18.x.x`, o Node.js foi instalado com sucesso.

---

## **4. Como o NVM e o Node.js Funcionam Juntos?**
- O **NVM** permite instalar várias versões do Node.js no mesmo sistema.
- Você pode alternar entre versões rapidamente usando:
  ```sh
  nvm use <versão>
  ```
- Para ver as versões instaladas localmente:
  ```sh
  nvm list
  ```
- Para remover uma versão antiga:
  ```sh
  nvm uninstall <versão>
  ```

Isso é útil para desenvolvedores que trabalham em projetos diferentes, pois cada projeto pode exigir uma versão específica do Node.js.

---

## **5. Diferenças entre NVM e nvm-windows**
| Recurso            | NVM (Linux/macOS) | NVM-Windows |
|-------------------|-----------------|------------|
| Instalação        | Script Bash      | Instalador `.exe` |
| Interface        | Terminal (Bash/Zsh) | Prompt de Comando (CMD) |
| Alternância de Versões | ✅ Sim          | ✅ Sim |
| Suporte Oficial  | ✅ Sim          | ❌ Não (projeto separado) |

Se você estiver no **Windows**, use o **nvm-windows**. Se estiver no **Linux/macOS**, use o **NVM oficial**.

---

## **6. Conclusão**
- O **Node.js** é essencial para desenvolvimento backend com JavaScript.
- O **NVM** facilita a instalação e troca entre versões do Node.js.
- No **Windows**, use o **nvm-windows**.
- No **Linux/macOS**, instale o **NVM oficial** via script.

Agora você pode gerenciar facilmente diferentes versões do Node.js para seus projetos! 🚀
Aqui está um **guia completo e detalhado** para instalar o **Poetry no Windows**, cobrindo todos os cenários e possíveis problemas.  

---

## 📌 **Pré-requisitos**
Antes de instalar o Poetry, verifique se você tem:  

1. **Python instalado** (versão 3.7 ou superior)  
   - Para verificar, execute no **Prompt de Comando (CMD)**:  
     ```powershell
     python --version
     ```
   - Se não tiver o Python, baixe e instale em:  
     👉 [https://www.python.org/downloads/windows/](https://www.python.org/downloads/windows/)  
   - **IMPORTANTE:** Durante a instalação, **marque a opção** ✅ *"Add Python to PATH"*  

2. **PowerShell atualizado**  
   - Para verificar a versão do PowerShell:  
     ```powershell
     $PSVersionTable.PSVersion
     ```
   - Se for inferior a 5.1, atualize-o em:  
     👉 [https://aka.ms/PSWindows](https://aka.ms/PSWindows)  

---

## 🛠️ **Método 1 – Instalação pelo Script Oficial (Recomendado)**
Este é o método oficial do Poetry.  

1️⃣ **Abra o PowerShell** como Administrador (**Importante!**)  
2️⃣ Execute o seguinte comando:  
   ```powershell
   (Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | python -
   ```
3️⃣ Aguarde a instalação terminar  
4️⃣ Feche o terminal e abra novamente  

### 🔹 **Verificar se a instalação foi bem-sucedida:**  
Execute:  
```powershell
poetry --version
```
Se aparecer algo como `Poetry 1.x.x`, a instalação foi bem-sucedida! 🎉  

---

## 🛠️ **Método 2 – Instalar via pip (Alternativa)**
Se preferir instalar usando o `pip`, siga este processo:  

1️⃣ Abra o **Prompt de Comando (CMD)** ou **PowerShell**  
2️⃣ Instale o Poetry via pip:  
   ```powershell
   pip install poetry
   ```
3️⃣ Verifique a instalação:  
   ```powershell
   poetry --version
   ```

---

## 🔧 **Adicionando o Poetry ao PATH (se necessário)**
Caso o comando `poetry` não seja reconhecido após a instalação, adicione o caminho do executável ao **PATH**:  

1️⃣ Localize a pasta onde o Poetry foi instalado. Normalmente, fica em:
   ```powershell
   %APPDATA%\Python\Scripts
   ```
2️⃣ **Adicione esse caminho ao PATH:**  
   - Abra o **Executar** (`Win + R`), digite `sysdm.cpl` e pressione **Enter**  
   - Vá até **"Avançado" → "Variáveis de ambiente"**  
   - Em **"Variáveis do sistema"**, edite `Path` e adicione:  
     ```
     %APPDATA%\Python\Scripts
     ```
   - Confirme e reinicie o terminal  

Agora, o comando `poetry` deve funcionar!  

---

## 🔍 **Possíveis Erros e Soluções**
### ❌ `poetry: command not found` ou `poetry não é reconhecido`
**Solução:**  
- Reinicie o terminal  
- Verifique se o **PATH** está configurado corretamente  
- Execute `python -m poetry --version` para testar a instalação  

### ❌ `python: command not found`
**Solução:**  
- Verifique se o Python está instalado e adicionado ao PATH  

---

## ✅ **Conclusão**
Agora você tem um guia **completo e detalhado** para instalar o Poetry no Windows. 🚀  
Se tiver alguma dúvida ou erro, me avise! 💬

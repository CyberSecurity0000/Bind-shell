<div align="center">

# 🐍 Python Bind Shell

**Projeto educacional em Python**

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Networking](https://img.shields.io/badge/Networking-TCP-2F81F7?style=for-the-badge&logo=socket&logoColor=white)
![Purpose](https://img.shields.io/badge/Purpose-Educational-8A2BE2?style=for-the-badge)

*Estudo de comunicação TCP, execução de processos e concorrência em Python.*

</div>

---

## 📌 Sobre

Implementação simples de uma **bind shell** para fins educacionais, explorando conceitos de redes e automação com Python.

## 🧠 Conceitos praticados

- 🌐 **Sockets TCP** — comunicação entre cliente e servidor.
- 📦 **Listas e `join()`** — acumular e reconstruir os dados recebidos.
- ⚙️ **`subprocess`** — executar processos e capturar a saída.
- 🧵 **Threads** — atender conexões de forma concorrente.
- 🎛️ **Click** — receber opções pela linha de comando.

## 🚀 Usage

> **Teste apenas em um laboratório isolado ou em `localhost`.** O servidor executa comandos recebidos pela conexão, sem autenticação.

### 1. Instale a dependência

```bash
python3 -m pip install click
```

### 2. Inicie o servidor

Salve o código como `bind_shell.py` e execute:

```bash
python3 bind_shell.py --port 4444
```

A porta padrão é `4444`, então `--port 4444` é opcional.

### 3. Conecte-se localmente

Em outro terminal da mesma máquina, use `netcat`:

```bash
nc 127.0.0.1 4444
```

Digite um comando de teste, como `whoami`, e pressione **Enter**. Para encerrar a sessão, digite `exit`.

## 🔄 Fluxo

`Aguardar conexão → Receber dados → Reconstruir comando → Executar → Enviar resposta`

## ⚠️ Aviso de segurança

> **Use somente em laboratório local ou em ambientes com autorização explícita.**
>
> O script executa comandos recebidos pela conexão e não implementa autenticação. Ele usa `0.0.0.0`, ou seja, escuta em todas as interfaces de rede; portanto, faça testes em ambiente isolado e bloqueie conexões externas. Os comandos são executados com as permissões do usuário que iniciou o programa. **Não o exponha à internet nem o utilize em sistemas sem autorização.** Este projeto é educacional e não foi desenvolvido para uso em produção.

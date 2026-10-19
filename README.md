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

## 🔄 Fluxo

`Aguardar conexão → Receber dados → Reconstruir comando → Executar → Enviar resposta`

## ⚠️ Aviso de segurança

> **Use somente em laboratório local ou em ambientes com autorização explícita.**
>
> O script executa comandos recebidos pela conexão e não implementa autenticação. **Não o exponha à internet nem o utilize em sistemas sem autorização.** Este projeto é educacional e não foi desenvolvido para uso em produção.

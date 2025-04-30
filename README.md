# 🎥 Sistema Inteligente de Monitoramento de Câmeras de Trânsito

Este repositório reúne um sistema colaborativo desenvolvido como parte do desafio de **Inteligência Artificial na automatização do sinal das câmeras de trânsito**, proposto durante a Residência do Porto Digital. A empresa parceira selecionada para este desafio foi a **Rede Globo**.

A solução permite monitorar câmeras de trânsito em tempo real e automatizar a troca de câmeras com base na narração ao vivo e no roteiro do editor, utilizando técnicas de Inteligência Artificial e Processamento de Linguagem Natural (PLN).

---

## 🎯 Objetivo do Projeto

- Automatizar a seleção de câmeras com base na fala do(a) apresentador(a).
- Exibir vídeos de trânsito em tempo real usando **streaming via HLS (MediaMTX)**.
- Integrar comandos de voz para navegação automática e fluida entre câmeras.
- Reduzir a intervenção manual dos operadores durante a exibição.

---

## 🤖 Onde a IA é Aplicada?

- **Reconhecimento de Voz:** captura e interpretação de comandos do(a) apresentador(a) em tempo real.
- **Processamento de Linguagem Natural (PLN):** interpretação inteligente de nomes de locais e comandos indiretos para identificar a câmera mais adequada.
- **Automação de Exibição:** exibe dinamicamente a câmera correspondente à narrativa jornalística com base nos comandos de voz detectados.

> 💡 **Exemplo:** ao ouvir "vamos agora para a Avenida Conde da Boa Vista", o sistema automaticamente alterna para a câmera da Boa Vista.

---

## 👨‍💻 Tecnologias e Bibliotecas Utilizadas

### 🎨 Interface Web

- **HTML5**, **CSS3**, **JavaScript Vanilla**
- **MediaMTX v1.12.0** – servidor de streaming RTSP/HLS
- **HLS.js** – player de vídeo para reprodução dos streams HLS

### 🧠 Inteligência Artificial / Reconhecimento de Voz
- **SpeechRecognition API** (navegadores compatíveis)
- **Web Speech API** – para comandos de voz e captura de fala
- **Custom Mapping e Normalização de Texto** – associação de comandos a câmeras com tolerância semântica

---

## 🛠️ Como Rodar o Projeto Localmente

### 1. Instale o MediaMTX
Faça o download [neste link](https://github.com/bluenviron/mediamtx/releases) e configure o arquivo `mediamtx.yml` com os streams RTSP das suas câmeras.

```bash
./mediamtx mediamtx.yml
```

Isso iniciará os servidores nas portas padrão:
- RTSP: `8554`
- HLS: `8888`

### 2. Inicie a Interface
Abra o arquivo `index.html` em seu navegador (**Google Chrome** recomendado).

---

## 🧩 Estrutura do Projeto

```
📦 monitoramento-transito/
├── mediamtx/                 # Configuração do servidor de streaming
│   └──  mediamtx.yml        
├── README.md                 # Documentação e instruções              
├── index.html                # Interface e lógica de controle por voz
└── logo_globo.png            # Logotipo da interface
```

---

## 🧪 Funcionalidades Implementadas

- ✅ Visualização da câmera principal em tela cheia.
- ✅ Lista lateral de câmeras com status online/offline.
- ✅ Alternância de câmeras por voz ou controle manual.
- ✅ Reconhecimento de voz ativável/desativável.
- ✅ Log de comandos e fallback automático para modo manual.

---

## 🗂️ Arquitetura da Solução

![Arquitetura do Sistema](arquitetura_monitoramento.svg)

---

## 🤝 Projeto em Equipe

Este projeto foi desenvolvido de forma colaborativa durante a **Residência do Porto Digital na Rede Globo** (Março 2025 – presente), com foco em soluções de automação aplicadas ao jornalismo e monitoramento urbano em tempo real.

---

## 📬 Contato

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/livialorrani/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/livialorrani)

---

> Projeto desenvolvido com ❤️ por um time dedicado à inovação no telejornalismo inteligente da Rede Globo.

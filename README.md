# GolpeGuard: Detetor Inteligente de Golpes com Flask, IA e Aprendizagem Contínua

Detecta mensagens fraudulentas com IA híbrida (modelo local + GPT-4 Turbo / Gemini Pro), aprendizado contínuo e integração via Flask API.

![Interface do GolpeGuard TI](./interface-golpeguard.png)

---

## 🔍 Funcionalidades Principais

- ✅ **Classificação Híbrida:** Modelo local com fallback para IA externas (GPT-4, Gemini) baseado em limiar de confiança.
- 🔁 **Aprendizagem Contínua:** Aprende com o feedback do usuário e com exemplos coletados automaticamente do ReclameAqui.
- ⚙️ **Retreinamento Automático:** Atualiza o modelo local periodicamente e após feedbacks.
- 📊 **Avaliação de Modelo:** Relatórios de desempenho gerados automaticamente.
- 🔐 **Segurança:** Uso de variáveis de ambiente para proteção de chaves API.
- 🌐 **API RESTful Versionada:** Endpoints organizados para classificação e retreinamento.
- 🚀 **Suporte a Google Colab:** Via pyngrok para testes remotos.

---

## 🚀 Como Executar

### Localmente
```bash
pip install -r requirements.txt
python app.py
```

### Google Colab
Execute o notebook `golpeguard_colab.ipynb` com ngrok habilitado.

---

## 📬 API Endpoints

- `POST /api/v1/classificar` – Classifica uma mensagem como golpe ou legítima.
- `POST /api/v1/retrain` – Retreina o modelo com novos dados (proteção recomendada).

---

## 🧠 Tecnologias Utilizadas

- Python + Flask
- Scikit-learn (Naive Bayes)
- OpenAI API (GPT-4 Turbo)
- Google Generative AI (Gemini Pro)
- BeautifulSoup & Requests (web scraping)
- Pyngrok (Colab)

---

## 📌 Objetivo

Este projeto visa criar um sistema acessível e eficiente para detecção de golpes em mensagens (SMS, WhatsApp, e-mails), combinando técnicas de IA local com inteligência artificial de última geração em nuvem.

---

## 👨‍💻 Autor

**Alexandre Freitas de Lima Pacheco**  
Estudante de Engenharia da Computação – IFPB Campus Campina Grande  

---

## 📄 Licença

Este projeto está licenciado sob a licença MIT.

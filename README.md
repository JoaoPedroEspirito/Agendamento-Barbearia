# 💈 BarberShop - Sistema de Agendamento Profissional

Este é o meu **Projeto de Final de Curso (PFC)** para o Bacharelado em Sistemas de Informação. É uma solução *full-stack* completa, focada na automação de agendamentos para barbearias, com foco em escalabilidade e deploy automatizado.

---

## 🔗 Links do Projeto (Live Demo)

* **Frontend (Vercel):** [https://agendamento-barbearia-lilac.vercel.app/](https://agendamento-barbearia-lilac.vercel.app/)
* **Backend & Swagger (Render):** [https://barbearia-api-apx9.onrender.com/swagger](https://barbearia-api-apx9.onrender.com/swagger)

---

## 🎯 Funcionalidades Principais

### **Área do Cliente**
* **Cadastro e Auth:** Registro seguro com validação de senha.
* **Agendamento Inteligente:** Escolha de barbeiro, serviço e horários disponíveis em tempo real.
* **Notificações:** Recebimento de e-mails de confirmação e cancelamento via **SendGrid**.

### **Painel Administrativo (Barbeiros/Admin)**
* **Gestão de Agenda:** Visualização centralizada de todos os compromissos.
* **Gerenciamento de Serviços:** CRUD completo de serviços e preços.
* **Controle de Horários:** Configuração de disponibilidade dos profissionais.

---

## 🛠️ Arquitetura e Tecnologias

O projeto utiliza uma arquitetura moderna e desacoplada:

* **Backend:** ASP.NET Core Web API (.NET 9) seguindo princípios de **Clean Code**.
* **Database:** PostgreSQL hospedado no **Supabase**.
* **Email:** SendGrid API para comunicação transacional.
* **DevOps:** Dockerizado e com pipeline de deploy contínuo no Render.

---

## 🔐 Variáveis de Ambiente

Para o projeto rodar (local ou nuvem), você precisa configurar as seguintes chaves:

| Variável | Descrição |
| :--- | :--- |
| `ConnectionStrings__AppDbConnection` | String de conexão (ADO.NET) do PostgreSQL/Supabase. |
| `SendGridApiKey` | Chave de API do SendGrid. |
| `SendGrid__FromEmail` | E-mail verificado como remetente no SendGrid. |
| `AdminSettings__Email` | E-mail inicial para o primeiro Administrador (Seeder). |
| `AdminSettings__Password` | Senha inicial para o primeiro Administrador (Seeder). |

---

## 🔧 Guia de Instalação Local

### 1. Clonar o Repositório
```bash
git clone [https://github.com/JoaoPedroEspirito/Agendamento-Barbearia.git](https://github.com/JoaoPedroEspirito/Agendamento-Barbearia.git)
cd Agendamento-Barbearia
```

### 2. Configurando o Backend
```bash
cd backend
# Restaura os pacotes e aplica as migrations
dotnet ef database update
dotnet run
```

### 3. Configurando o Frontend
```bash
cd frontend
npm install
npm start
```

---

## 👨‍💻 Autor

**João Pedro Araujo do Espirito Santo**

```

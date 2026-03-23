# TVDE Finance v2

Aplicação full-stack para gerenciamento financeiro com dashboard de ganhos/despesas, trip logger, expense tracker, community feed e painel admin.

## Stack Tecnológico

- **Frontend:** Vite, React 18, TypeScript, Tailwind CSS
- **Backend:** Firebase (Firestore, Authentication)
- **Autenticação:** Google Sign-In (obrigatório)
- **Hosting:** Vercel
- **CI/CD:** GitHub Actions

## Requisitos

- Node.js 18+
- npm ou pnpm
- Conta Firebase com projeto configurado
- Conta GitHub para CI/CD

## Instalação

1. Clone o repositório:
```bash
git clone https://github.com/transferleiria-ctrl/tvde-finance-v2
cd tvde-finance-v2
```

2. Instale as dependências:
```bash
pnpm install
```

3. Crie um arquivo `.env.local` com as variáveis de ambiente do Firebase:
```
VITE_FIREBASE_API_KEY=sua_api_key
VITE_FIREBASE_AUTH_DOMAIN=seu_auth_domain
VITE_FIREBASE_PROJECT_ID=seu_project_id
VITE_FIREBASE_STORAGE_BUCKET=seu_storage_bucket
VITE_FIREBASE_MESSAGING_SENDER_ID=seu_messaging_sender_id
VITE_FIREBASE_APP_ID=seu_app_id
```

## Desarrollo

```bash
pnpm dev
```

A aplicação estará disponível em `http://localhost:5173`.

## Build para Produção

```bash
pnpm build
```

## Funcionalidades

- **Dashboard:** Resumo de ganhos, despesas e saldo
- **Trip Logger:** Registrar viagens com ganhos, km e tempo
- **Expense Tracker:** Rastrear despesas (combustível, manutenção, seguro, portagens)
- **Financial Reports:** Gráficos e estatísticas
- **Community Feed:** Posts de dicas e recomendações
- **Leaderboard:** Ranking de motoristas por ganhos
- **Admin Panel:** Gerenciamento de usuários e dados

## Configuração do Firebase

1. Crie um projeto no [Firebase Console](https://console.firebase.google.com/)
2. Habilite Google Authentication
3. Crie um banco de dados Firestore em modo produção
4. Configure as regras de segurança conforme `firestore.rules`
5. Configure o Firebase Storage conforme `storage.rules`

## Deployment no Vercel

1. Conecte o repositório GitHub ao Vercel
2. Configure as variáveis de ambiente do Firebase no dashboard do Vercel
3. Deploy automático será acionado a cada push em main

## Admin Email

Email de administrador: `carloslucaspt2023@gmail.com`

## License

MIT

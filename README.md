# Lucid Lease Studio

🏢 Plataforma inteligente de gerenciamento de aluguéis com dashboard avançado e analytics em tempo real.

## 📋 Descrição

O **Lucid Lease Studio** é uma solução completa e intuitiva para gerenciamento de propriedades e aluguéis, oferecendo uma interface moderna e poderosa para proprietários, administradores e inquilinos. Com foco na experiência do usuário e analytics avançados, a plataforma simplifica todo o processo de gestão imobiliária.

## ✨ Principais Funcionalidades

### 🎯 Para Proprietários
- **Dashboard Intuitivo**: Visão geral completa de todas as propriedades
- **Gestão de Contratos**: Criação, edição e acompanhamento de contratos
- **Relatórios Financeiros**: Analytics detalhados de receitas e despesas
- **Manutenção**: Sistema de ordens de serviço e acompanhamento
- **Comunicação**: Chat integrado com inquilinos

### 🏠 Para Inquilinos
- **Portal do Inquilino**: Acesso a informações do contrato e propriedade
- **Pagamentos Online**: Sistema seguro de pagamento de aluguéis
- **Solicitações**: Abertura de tickets para manutenção e suporte
- **Documentos**: Acesso a contratos e comprovantes

### 📊 Analytics e Relatórios
- **Métricas em Tempo Real**: Ocupação, receitas, inadimplência
- **Análise de Tendências**: Insights sobre o mercado imobiliário
- **Relatórios Customizáveis**: Exportação de dados em múltiplos formatos
- **Alertas Inteligentes**: Notificações automáticas para eventos importantes

## 🚀 Tecnologias Utilizadas

- **[React](https://reactjs.org/)** - Biblioteca JavaScript para interfaces reativas
- **[TypeScript](https://www.typescriptlang.org/)** - Superset do JavaScript com tipagem estática
- **[Vite](https://vitejs.dev/)** - Build tool moderna e ultra-rápida
- **[Tailwind CSS](https://tailwindcss.com/)** - Framework CSS utilitário
- **[shadcn/ui](https://ui.shadcn.com/)** - Componentes de UI modernos e acessíveis
- **[Recharts](https://recharts.org/)** - Biblioteca de gráficos para React
- **[React Hook Form](https://react-hook-form.com/)** - Formulários performáticos
- **[Zustand](https://github.com/pmndrs/zustand)** - Gerenciamento de estado simples
- **[React Query](https://tanstack.com/query)** - Sincronização e cache de dados
- **[Framer Motion](https://www.framer.com/motion/)** - Animações fluidas

## 📦 Pré-requisitos

Certifique-se de ter instalado:

- **Node.js** (versão 18 ou superior)
- **npm** ou **yarn** ou **pnpm**

### Instalação do Node.js com NVM

```bash
# Instalar NVM
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash

# Reiniciar terminal e instalar Node.js
nvm install node
nvm use node
```

## 🛠️ Instalação e Configuração

### Método 1: Desenvolvimento Local

```bash
# 1. Clone o repositório
git clone https://github.com/feliciocavalcante/lucid-lease-studio.git

# 2. Navegue até o diretório
cd lucid-lease-studio

# 3. Instale as dependências
npm install

# 4. Configure as variáveis de ambiente
cp .env.example .env.local

# 5. Inicie o servidor de desenvolvimento
npm run dev
```


### Método 2: GitHub Codespaces

1. Vá para a página principal do repositório
2. Clique no botão **"Code"** (verde)
3. Selecione **"Codespaces"**
4. Clique em **"New codespace"**
5. Desenvolva diretamente no browser

## ⚙️ Configuração do Ambiente

Crie um arquivo `.env.local` na raiz do projeto:

```env
# API Configuration
VITE_API_BASE_URL=http://localhost:3000/api
VITE_APP_NAME=Lucid Lease Studio

# Environment
VITE_NODE_ENV=development

# Authentication
VITE_AUTH_DOMAIN=your-auth-domain.com
VITE_AUTH_CLIENT_ID=your-client-id

# File Upload
VITE_CLOUDINARY_CLOUD_NAME=your-cloud-name
VITE_UPLOAD_PRESET=your-upload-preset

# Maps (opcional)
VITE_GOOGLE_MAPS_API_KEY=your-maps-api-key

# Analytics (opcional)
VITE_GA_TRACKING_ID=GA-XXXXXXXXX

# Feature Flags
VITE_ENABLE_CHAT=true
VITE_ENABLE_PAYMENTS=true
VITE_ENABLE_MAINTENANCE=true
```

## 📝 Scripts Disponíveis

```bash
# Desenvolvimento com hot reload
npm run dev

# Build para produção
npm run build

# Preview do build de produção
npm run preview

# Executar testes
npm run test

# Testes em modo watch
npm run test:watch

# Coverage dos testes
npm run test:coverage

# Lint do código
npm run lint

# Correção automática de lint
npm run lint:fix

# Formatação de código
npm run format

# Análise de bundle
npm run analyze

# Tipo checking
npm run type-check
```

## 🏗️ Estrutura do Projeto

```
lucid-lease-studio/
├── public/                    # Arquivos estáticos
│   ├── icons/                # Ícones da aplicação
│   └── images/               # Imagens públicas
├── src/                      # Código fonte
│   ├── components/           # Componentes reutilizáveis
│   │   ├── ui/              # Componentes base (shadcn/ui)
│   │   ├── charts/          # Componentes de gráficos
│   │   ├── forms/           # Formulários
│   │   └── layout/          # Componentes de layout
│   ├── pages/               # Páginas da aplicação
│   │   ├── dashboard/       # Dashboard principal
│   │   ├── properties/      # Gestão de propriedades
│   │   ├── tenants/         # Gestão de inquilinos
│   │   ├── contracts/       # Gestão de contratos
│   │   ├── financial/       # Relatórios financeiros
│   │   └── settings/        # Configurações
│   ├── hooks/               # Custom hooks
│   ├── services/            # Serviços e APIs
│   ├── stores/              # Gerenciamento de estado
│   ├── types/               # Definições TypeScript
│   ├── utils/               # Utilitários
│   ├── styles/              # Estilos globais
│   └── constants/           # Constantes da aplicação
├── tests/                   # Testes
├── docs/                    # Documentação
├── package.json
├── tailwind.config.js       # Configuração Tailwind
├── tsconfig.json           # Configuração TypeScript
├── vite.config.ts          # Configuração Vite
└── README.md
```

## 🎨 Design System

### Cores e Temas

```css
/* Tema Claro */
--primary: 220 90% 56%        /* Azul principal */
--secondary: 220 14% 96%      /* Cinza secundário */
--accent: 142 71% 45%         /* Verde accent */
--success: 142 71% 45%        /* Verde sucesso */
--warning: 38 92% 50%         /* Amarelo aviso */
--error: 0 84% 60%            /* Vermelho erro */

/* Tema Escuro */
--primary: 220 90% 56%
--secondary: 220 13% 18%
--accent: 142 71% 45%
```

### Componentes Base

- **Buttons**: Variações primary, secondary, outline, ghost
- **Cards**: Containers com sombras e bordas arredondadas
- **Forms**: Inputs, selects, checkboxes estilizados
- **Tables**: Tabelas responsivas com sorting
- **Modals**: Overlays e dialogs
- **Charts**: Gráficos interativos e responsivos

## 📊 Funcionalidades Principais

### Dashboard Analytics

```typescript
// Métricas principais
interface DashboardMetrics {
  totalProperties: number;
  occupancyRate: number;
  monthlyRevenue: number;
  maintenanceRequests: number;
  overduePayments: number;
}

// Gráficos disponíveis
- Revenue Trends (Linha)
- Occupancy Rate (Donut)
- Property Distribution (Bar)
- Payment Status (Pie)
- Maintenance Timeline (Area)
```

### Gestão de Propriedades

- **CRUD Completo**: Criar, editar, visualizar e arquivar propriedades
- **Upload de Imagens**: Galeria de fotos com drag & drop
- **Geolocalização**: Integração com mapas
- **Documentos**: Upload e gestão de documentos
- **Histórico**: Timeline de alterações

### Sistema de Contratos

- **Templates**: Modelos de contrato personalizáveis
- **Assinatura Digital**: Integração com provedores de e-signature
- **Renovações**: Alertas automáticos e workflow de renovação
- **Aditivos**: Gestão de alterações contratuais

### Portal Financeiro

- **Fluxo de Caixa**: Entradas e saídas detalhadas
- **Previsões**: Projeções baseadas em contratos
- **Relatórios**: Múltiplos formatos de exportação
- **Integração Bancária**: Conciliação automática

## 🔒 Autenticação e Segurança

### Sistema de Roles

```typescript
enum UserRole {
  SUPER_ADMIN = 'super_admin',
  PROPERTY_MANAGER = 'property_manager',
  LANDLORD = 'landlord',
  TENANT = 'tenant'
}

// Permissões por role
interface Permissions {
  canManageProperties: boolean;
  canViewFinancials: boolean;
  canManageUsers: boolean;
  canAccessAnalytics: boolean;
}
```

### Segurança

- **JWT Authentication**: Tokens seguros com refresh
- **RBAC**: Controle de acesso baseado em roles
- **2FA**: Autenticação de dois fatores (opcional)
- **Audit Log**: Registro de todas as ações importantes
- **HTTPS**: Comunicação criptografada

## 📱 Responsividade

O Lucid Lease Studio é totalmente responsivo:

- **Desktop**: Layout completo com sidebar e múltiplas colunas
- **Tablet**: Adaptação inteligente dos componentes
- **Mobile**: Interface otimizada para touch
- **PWA**: Funciona como app nativo (opcional)

### Breakpoints

```css
/* Tailwind CSS breakpoints */
sm: 640px    /* Smartphone landscape */
md: 768px    /* Tablet portrait */
lg: 1024px   /* Tablet landscape */
xl: 1280px   /* Desktop */
2xl: 1536px  /* Large desktop */
```

## 🧪 Testes

```bash
# Executar todos os testes
npm run test

# Testes com watch mode
npm run test:watch

# Coverage report
npm run test:coverage

# Testes e2e (se configurado)
npm run test:e2e
```

### Estrutura de Testes

```
tests/
├── unit/                    # Testes unitários
│   ├── components/
│   ├── hooks/
│   └── utils/
├── integration/             # Testes de integração
├── e2e/                     # Testes end-to-end
├── fixtures/                # Dados de teste
└── setup.ts                 # Configuração
```

## 🚀 Deploy e Publicação

### Deploy Automático via Lovable

1. Acesse o [Projeto no Lovable](https://lovable.dev/projects/cc3344c1-cad8-42de-9061-3d8412053833)
2. Clique em **Share** → **Publish**
3. Sua aplicação estará live instantaneamente

### Configurar Domínio Personalizado

1. Vá para **Project** → **Settings** → **Domains**
2. Clique em **Connect Domain**
3. Siga as instruções para conectar seu domínio

📖 [Guia completo de configuração de domínio](https://docs.lovable.dev/tips-tricks/custom-domain#step-by-step-guide)

### Deploy Manual

```bash
# Build de produção
npm run build

# Os arquivos estarão em /dist
# Deploy para qualquer provedor:
# - Vercel: vercel --prod
# - Netlify: netlify deploy --prod
# - AWS S3: aws s3 sync dist/ s3://bucket-name
```

## 📈 Performance

### Otimizações Implementadas

- **Code Splitting**: Carregamento lazy de rotas
- **Tree Shaking**: Eliminação de código não utilizado
- **Image Optimization**: Lazy loading e WebP
- **Bundle Analysis**: Monitoramento do tamanho
- **Caching**: Estratégias de cache inteligentes

### Métricas Alvo

- **First Contentful Paint**: < 1.5s
- **Largest Contentful Paint**: < 2.5s
- **Cumulative Layout Shift**: < 0.1
- **First Input Delay**: < 100ms

## 🔧 Configurações Avançadas

### Customização de Tema

```typescript
// tailwind.config.js
module.exports = {
  theme: {
    extend: {
      colors: {
        brand: {
          50: '#eff6ff',
          500: '#3b82f6',
          900: '#1e3a8a',
        }
      },
      fontFamily: {
        sans: ['Inter', 'sans-serif'],
      }
    }
  }
}
```

### Plugins e Extensões

- **React Query DevTools**: Debug de requisições
- **Storybook**: Documentação de componentes
- **Bundle Analyzer**: Análise de performance
- **ESLint + Prettier**: Qualidade de código

## 🤝 Contribuindo

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-funcionalidade`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova funcionalidade'`)
4. Push para a branch (`git push origin feature/nova-funcionalidade`)
5. Abra um Pull Request

### Padrões de Código

```bash
# Antes de commitar
npm run lint        # Verificar padrões
npm run format      # Formatar código
npm run type-check  # Verificar tipos
npm run test        # Executar testes
```

### Convenções

- **Commits**: Use [Conventional Commits](https://www.conventionalcommits.org/)
- **Components**: PascalCase (ex: `PropertyCard`)
- **Hooks**: Prefixo `use` (ex: `usePropertyData`)
- **Constants**: UPPER_SNAKE_CASE
- **Files**: kebab-case para arquivos, PascalCase para componentes

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👨‍💻 Autor

**Felício Cavalcante**
- GitHub: [@feliciocavalcante](https://github.com/feliciocavalcante)

## 🆘 Suporte

Precisa de ajuda? Temos várias opções:

1. **Issues**: [GitHub Issues](https://github.com/feliciocavalcante/lucid-lease-studio/issues)
2. **Discussões**: [GitHub Discussions](https://github.com/feliciocavalcante/lucid-lease-studio/discussions)
3. **Documentação**: [Wiki do Projeto](https://github.com/feliciocavalcante/lucid-lease-studio/wiki)
4. **Lovable**: [Documentação Oficial](https://docs.lovable.dev/)

## 🗺️ Roadmap

### 🎯 Próximas Funcionalidades

- [ ] **Mobile App**: Aplicativo nativo React Native
- [ ] **IA Integration**: Sugestões inteligentes de preços
- [ ] **Multi-idioma**: Suporte a português, inglês e espanhol
- [ ] **API Pública**: Endpoints para integrações terceiras
- [ ] **Marketplace**: Plataforma de busca de imóveis
- [ ] **IoT Integration**: Sensores e automação residencial

### 🔮 Visão de Longo Prazo

- **Blockchain**: Contratos inteligentes para aluguéis
- **VR Tours**: Tours virtuais das propriedades
- **Sustentabilidade**: Métricas ambientais
- **Social Features**: Rede social para inquilinos

## 📊 Analytics e Métricas

### Dashboard Principal

- **Propriedades Ativas**: Total de imóveis sob gestão
- **Taxa de Ocupação**: Percentual de ocupação em tempo real
- **Receita Mensal**: Faturamento do mês corrente
- **Inadimplência**: Percentual de pagamentos em atraso
- **Tickets Abertos**: Solicitações de manutenção pendentes

### Relatórios Disponíveis

- **Financeiro**: Receitas, despesas e fluxo de caixa
- **Operacional**: Ocupação, rotatividade e manutenção
- **Analítico**: Trends de mercado e benchmarks
- **Personalizado**: Relatórios sob medida

---

⭐ **Se este projeto te impressionou, considere deixar uma estrela!**

🚀 **Pronto para revolucionar seu negócio imobiliário? Comece agora!**

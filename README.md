# Default Automation Frontend

A modern web application built with Next.js 15.2.4, TypeScript, and Tailwind CSS, providing a comprehensive dashboard for automation management across different user roles.

## Features

- 🔐 Multi-role authentication (Admin, Partner, Visitor)
- 📊 Analytics dashboard with interactive charts
- 👥 User management and role assignments
- 📝 Blog and post management
- 🤖 Bot management and automation
- 🎯 Engagement tracking
- 📈 Leaderboard system
- 📜 Activity logging
- 🔔 Notification system
- 🎁 Rewards management
- ⚙️ System settings
- 🪤 Trap management
- 🎨 Responsive UI with dark mode support

## Prerequisites

- Node.js 18.x or later
- pnpm 8.x or later
- Docker and Docker Compose (for containerized deployment)

## Quick Start

1. Clone the repository:
   ```bash
   git clone [repository-url]
   cd default-automation-fe
   ```

2. Install dependencies:
   ```bash
   pnpm install
   ```

3. Create a `.env.local` file:
   ```bash
   cp .env.example .env.local
   ```

4. Start the development server:
   ```bash
   pnpm dev
   ```

Visit `http://localhost:3000` to access the application.

## Development

### Project Structure

```
default-automation-fe/
├── app/                    # Next.js 15.2.4 app directory
│   ├── admin/             # Admin role pages
│   ├── partner/           # Partner role pages
│   ├── visitor/           # Visitor role pages
│   └── login/             # Authentication pages
├── components/            # Reusable React components
│   └── ui/               # UI component library
├── lib/                   # Utility functions and API clients
├── public/               # Static assets
├── styles/              # Global styles and Tailwind config
└── types/               # TypeScript type definitions
```

### Available Scripts

- `pnpm dev` - Start development server
- `pnpm build` - Create production build
- `pnpm start` - Start production server
- `pnpm lint` - Run ESLint
- `pnpm type-check` - Run TypeScript type checking

## Docker Deployment

### Development

```bash
docker compose -f docker-compose.dev.yml up
```

### Production

```bash
docker compose up -d
```

See [deployment documentation](./docs/deployment.md) for more details.

## Environment Variables

| Variable | Description | Default |
|----------|-------------|---------|
| `NEXT_PUBLIC_API_URL` | Backend API URL | `http://localhost:8000` |
| `NEXT_PUBLIC_APP_URL` | Frontend App URL | `http://localhost:3000` |

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/my-feature`
3. Commit changes: `git commit -am 'Add my feature'`
4. Push to branch: `git push origin feature/my-feature`
5. Submit a pull request

## License

[MIT License](LICENSE)
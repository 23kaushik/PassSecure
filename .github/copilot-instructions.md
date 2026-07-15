# Blockchain Password Manager - Development Instructions

This document contains setup and development guidelines for the blockchain-based smart password manager project.

## Project Setup Checklist

- [x] Project directories created
- [ ] Frontend initialized
- [ ] Backend initialized
- [ ] Smart contracts initialized
- [ ] All dependencies installed
- [ ] Development server running

## Development Guidelines

### Code Style
- Use ES6+ features
- Follow React hooks best practices
- Use Tailwind CSS utility classes
- Keep components small and focused

### File Organization
- Components in `src/components/`
- Pages in `src/pages/`
- Utilities in `src/utils/`
- API calls in `src/services/`

### Naming Conventions
- React components: PascalCase
- Functions/variables: camelCase
- Constants: UPPER_SNAKE_CASE
- Files: same as exported component

### Git Workflow
- Feature branches: `feature/description`
- Bugfix branches: `fix/description`
- Commit messages: descriptive and concise

## Testing
- Unit tests for utility functions
- Component tests for React components
- API integration tests
- Smart contract tests with Hardhat

## Deployment

### Frontend
- Build: `npm run build`
- Deploy to Vercel/Netlify

### Backend
- Deploy to Heroku/Railway
- Set environment variables
- Configure MongoDB Atlas

### Smart Contracts
- Deploy to testnet first
- Verify on Etherscan
- Mainnet deployment checklist

## Environment Variables

### Frontend (.env.local)
```
VITE_API_URL=http://localhost:5000
VITE_CONTRACT_ADDRESS=0x...
VITE_WEB3_PROVIDER=http://localhost:8545
```

### Backend (.env)
```
PORT=5000
MONGODB_URI=mongodb://...
JWT_SECRET=your-secret-key
WEB3_PROVIDER=http://localhost:8545
```

## Troubleshooting

- Clear node_modules and reinstall if dependency issues occur
- Ensure ports 5173 (frontend), 5000 (backend) are available
- Check MetaMask wallet is connected to correct network

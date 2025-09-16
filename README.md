# React + TypeScript + Vite + Tailwind CSS 4 + Biome

A modern, fast, and opinionated React development template with the latest tools and best practices.

## 🚀 Tech Stack

- **[Vite](https://vitejs.dev/)** - Next generation frontend tooling
- **[React 19](https://react.dev/)** - UI library with latest features
- **[TypeScript](https://www.typescriptlang.org/)** - Type-safe JavaScript
- **[Tailwind CSS 4](https://tailwindcss.com/)** - Utility-first CSS framework
- **[Biome](https://biomejs.dev/)** - Fast formatter and linter
- **[Bun](https://bun.sh/)** - Fast JavaScript runtime and package manager

## ✨ Features

- ⚡ **Vite** for lightning-fast development and builds
- ⚛️ **React 19** with SWC for optimal performance
- 🎨 **Tailwind CSS 4** with Vite plugin for instant styling
- 🔧 **Biome** for code formatting and linting (replaces ESLint + Prettier)
- 📦 **Bun** for fast package management
- 🎯 **TypeScript** for type safety
- 🔄 **Hot Module Replacement (HMR)** for instant updates
- 📱 **Responsive design** ready
- 🎨 **Modern CSS utilities** with `clsx` and `tailwind-merge`

## 🛠️ Development

### Prerequisites

- [Bun](https://bun.sh/) (recommended) or Node.js 18+
- Modern code editor (VS Code recommended)
- **Biome VS Code Extension** - Install the [Biome extension](https://marketplace.visualstudio.com/items?itemName=biomejs.biome) for real-time linting and formatting

### Getting Started

1. **Clone and install dependencies:**
   ```bash
   bun install
   ```

2. **Start the development server:**
   ```bash
   bun run dev
   ```

3. **Open your browser:**
   Navigate to `http://localhost:5173`

### Available Scripts

```bash
# Development
bun run dev          # Start development server with HMR

# Building
bun run build        # Build for production
bun run preview      # Preview production build

# Code Quality
bun run lint         # Run type checking and linting
bun run lint:fix     # Fix linting issues automatically
bun run format       # Format code with Biome
bun run check        # Run all checks and fixes
```

## 🎨 Styling with Tailwind CSS 4

This project uses **Tailwind CSS 4** with the new Vite plugin for optimal performance:

```tsx
// Example component with Tailwind classes
function Button({ variant = 'primary', children, ...props }) {
  return (
    <button
      className={clsx(
        'px-4 py-2 rounded-lg font-medium transition-colors',
        {
          'bg-blue-600 text-white hover:bg-blue-700': variant === 'primary',
          'bg-gray-200 text-gray-900 hover:bg-gray-300': variant === 'secondary',
        }
      )}
      {...props}
    >
      {children}
    </button>
  );
}
```

### Tailwind CSS 4 Features

- **Zero-config setup** - Works out of the box
- **Vite integration** - Optimized for fast builds
- **Modern CSS** - Uses latest CSS features
- **Utility classes** - Rapid UI development
- **Responsive design** - Mobile-first approach

## 🔧 Code Quality with Biome

This project uses **Biome** instead of ESLint + Prettier for:

- ⚡ **Faster** - 10-100x faster than ESLint
- 🎯 **All-in-one** - Linting + formatting in one tool
- 🔧 **Zero config** - Works out of the box
- 📦 **Smaller** - Single dependency

### Biome Configuration

The project includes a comprehensive Biome configuration in `biome.json`:

- **React-specific rules** for component best practices
- **TypeScript support** with type-aware linting
- **Accessibility rules** for better UX
- **Performance optimizations** for React apps
- **Tailwind CSS integration** with class sorting

### Running Biome

```bash
# Check for issues
bun run lint

# Fix issues automatically
bun run lint:fix

# Format code
bun run format

# Run all checks and fixes
bun run check
```

## 📁 Project Structure

```
src/
├── App.tsx          # Main application component
├── main.tsx         # Application entry point
├── index.css        # Global styles and Tailwind imports
└── vite-env.d.ts    # Vite type definitions
```

## 🚀 Deployment

### Build for Production

```bash
bun run build
```

The build artifacts will be stored in the `dist/` directory.

### Preview Production Build

```bash
bun run preview
```

## 🎯 Best Practices

### Component Development

- Use **TypeScript** for all components
- Follow **React 19** patterns and hooks
- Use **Tailwind CSS** for styling
- Keep components **small and focused**
- Use **Biome** for consistent code style

### Performance

- Leverage **Vite's** fast HMR for development
- Use **React 19** features like concurrent rendering
- Optimize with **Tailwind CSS 4** utility classes
- Run **Biome checks** before commits

### Code Quality

- **Install Biome VS Code Extension** - Get real-time linting and formatting
- Enable **Biome** in your editor settings
- Use **TypeScript** strict mode
- Follow **React** best practices
- Write **accessible** components

## 🔗 Useful Links

- [Vite Documentation](https://vitejs.dev/)
- [React Documentation](https://react.dev/)
- [Tailwind CSS Documentation](https://tailwindcss.com/)
- [Biome Documentation](https://biomejs.dev/)
- [TypeScript Documentation](https://www.typescriptlang.org/)

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

**Happy coding!** 🎉
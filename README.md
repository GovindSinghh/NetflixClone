# Netflix Clone

A static HTML/CSS/JavaScript Netflix clone website with a fully automated CI/CD pipeline.

## Features

- 🎬 Netflix-style UI with movie posters and banner
- 📱 Responsive design
- ⚡ Smooth scroll-based navigation effects
- 🚀 Fully automated CI/CD pipeline

## CI/CD Pipeline

This project includes a comprehensive CI/CD pipeline that automatically:

### 🔍 **Code Validation**
- **HTML Validation**: Uses HTMLHint to check HTML syntax and structure
- **CSS Validation**: Validates CSS syntax and structure
- **JavaScript Validation**: Lints JavaScript code with JSHint (ES6 compatible)
- **File Structure Check**: Ensures all required files are present

### 🔬 **Quality Assurance**
- **Lighthouse Audit**: Performance, accessibility, and SEO analysis
- **Automated Testing**: Runs on every push and pull request

### 🚀 **Deployment**
- **GitHub Pages**: Automatically deploys to GitHub Pages on main branch
- **Live Website**: Available at the GitHub Pages URL

## Getting Started

### Prerequisites
- Node.js 18+ (for development tools)
- Git

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/GovindSinghh/NetflixClone.git
   cd NetflixClone
   ```

2. **Install development dependencies**
   ```bash
   npm install
   ```

3. **Start local development server**
   ```bash
   npm run serve
   ```
   Visit http://localhost:8080 to view the website

4. **Run validation checks**
   ```bash
   npm run validate
   ```

### Available Scripts

- `npm run validate` - Run all validation checks
- `npm run validate:html` - Validate HTML files
- `npm run validate:css` - Validate CSS files  
- `npm run validate:js` - Validate JavaScript files
- `npm run serve` - Start local development server
- `npm test` - Run all tests (alias for validate)

## CI/CD Workflow

The pipeline runs automatically on:
- Push to `main` or `master` branch
- Pull requests to `main` or `master` branch

### Workflow Steps

1. **Setup Environment**
   - Checkout code
   - Setup Node.js 18
   - Install dependencies

2. **Code Validation**
   - HTML validation with HTMLHint
   - CSS syntax validation
   - JavaScript linting with JSHint
   - File structure verification

3. **Quality Audit**
   - Lighthouse performance audit
   - Accessibility testing
   - SEO analysis

4. **Deployment** (main branch only)
   - Deploy to GitHub Pages
   - Update live website

## Project Structure

```
NetflixClone/
├── .github/
│   └── workflows/
│       └── ci-cd.yml          # CI/CD pipeline configuration
├── images/                    # Movie posters and assets
│   ├── banner.jpg
│   ├── netflix-logo.png
│   ├── netflix-avatar.png
│   └── *.jpg                  # Movie poster images
├── index.html                 # Main HTML file
├── style.css                  # CSS styles
├── package.json               # Project configuration and scripts
├── .htmlhintrc               # HTML validation rules
├── .jshintrc                 # JavaScript linting rules
├── .gitignore                # Git ignore rules
└── README.md                 # This file
```

## Configuration Files

- **`.htmlhintrc`**: HTMLHint configuration for HTML validation
- **`.jshintrc`**: JSHint configuration for JavaScript linting
- **`.gitignore`**: Excludes node_modules and temporary files
- **`package.json`**: NPM scripts and dependencies

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Ensure all validations pass: `npm run validate`
5. Test locally: `npm run serve`
6. Submit a pull request

The CI/CD pipeline will automatically validate your changes!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

**GovindSinghh** - [GitHub Profile](https://github.com/GovindSinghh)

---

Built with ❤️ and automated with GitHub Actions 🚀
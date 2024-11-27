# Zaltadmin-Dashboard

Applications using Reactjs

## Preview

![screenshot20241127190814](https://github.com/user-attachments/assets/7a37752a-4e3b-47fb-aefb-887a0537ad25)

### 1. **Environment**
- **Node.js** (new version): [Download di sini](https://nodejs.org)
- **React Icons** : [Installation here](https://react-icons.github.io/react-icons/)
- **Tailwindcss** : [Installation here](https://tailwindcss.com/docs/guides/vite)

### 2. **Clone Repository**
Clone repository :
```bash
https://github.com/yogimp/Zaltadmin-Dashboard.git
```
Change directory:
```bash
cd Zaltadmin-Dashboard
```

### 3. **Dependency Installation**
Run the following command to install all required dependencies :
```bash
npm install
```

**Settingup**
If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:
- Configure the top-level `parserOptions` property like this:
  ```js
  export default tseslint.config({
    languageOptions: {
      // other options...
      parserOptions: {
        project: ['./tsconfig.node.json', './tsconfig.app.json'],
        tsconfigRootDir: import.meta.dirname,
      },
    },
  })
  ```

---
- Replace `tseslint.configs.recommended` to `tseslint.configs.recommendedTypeChecked` or `tseslint.configs.strictTypeChecked`
- Optionally add `...tseslint.configs.stylisticTypeChecked`
- Install eslint-plugin-react and update the config:

  ```js
  // eslint.config.js
  import react from 'eslint-plugin-react'
  
  export default tseslint.config({
    // Set the react version
    settings: { react: { version: '18.3' } },
    plugins: {
      // Add the react plugin
      react,
    },
    rules: {
      // other rules...
      // Enable its recommended rules
      ...react.configs.recommended.rules,
      ...react.configs['jsx-runtime'].rules,
    },
  })
  ```

### 4. **Run App**
Run the following command :
```bash
npm run dev
```

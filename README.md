# nikx-ui

<!-- Badges -->
<p align="left">
  <a href="https://www.npmjs.com/package/nikx-ui">
    <img src="https://img.shields.io/npm/v/nikx-ui?style=flat-square" alt="npm version" />
  </a>
  <a href="https://www.npmjs.com/package/nikx-ui">
    <img src="https://img.shields.io/npm/dm/nikx-ui?style=flat-square" alt="npm downloads" />
  </a>
  <a href="https://github.com/nikxpro/nikx-ui/blob/main/LICENSE">
    <img src="https://img.shields.io/npm/l/nikx-ui?style=flat-square" alt="license" />
  </a>
  <img src="https://img.shields.io/node/v/nikx-ui?style=flat-square" alt="node version" />
</p>

Reusable React component library for modern web applications.

## ✨ Features

- Customizable UI components
- Written in TypeScript
- Easy to style with SCSS variables

## 📦 Installation

```sh
pnpm install nikx-ui
```

<details>
<summary>Other package managers</summary>

```sh
npm install nikx-ui
# or
yarn add nikx-ui
```

</details>

## 🚀 Usage

### Import components

```tsx
import {
  Button,
  Input,
  Select,
  Table,
  TableBody,
  TableCell,
  TableHead,
  TableHeader,
  TableRow,
  TableFooter,
  TableCaption,
} from "nikx-ui";
```

### Import styles

```js
import "nikx-ui/dist/styles/main.css";
```

### Button Example

```tsx
<Button variant="primary" size="medium" onClick={() => alert("Clicked!")}>
  Click me
</Button>
```

### Input Example

```tsx
<Input
  label="Name"
  placeholder="Enter your name"
  value={value}
  onChange={handleChange}
  error={errorMsg}
/>
```

### Select Example

```tsx
<Select
  label="Country"
  options={[
    { value: "fr", label: "France" },
    { value: "us", label: "USA" },
  ]}
  value={selected}
  onChange={handleSelect}
  placeholder="Choose a country"
  error={errorMsg}
/>
```

### Table Example

```tsx
<Table>
  <TableHeader>
    <TableRow>
      <TableHead>Header 1</TableHead>
      <TableHead>Header 2</TableHead>
    </TableRow>
  </TableHeader>
  <TableBody>
    <TableRow>
      <TableCell>Cell 1</TableCell>
      <TableCell>Cell 2</TableCell>
    </TableRow>
  </TableBody>
</Table>
```

## 🎨 Theming

You can customize the look and feel by overriding SCSS variables before importing the main stylesheet:

```scss
$primary-color: #ff6600;
@import "nikx-ui/dist/styles/main.css";
```

See `src/styles/_variables.scss` for all available variables.

## 🤝 Contributing

1. Clone the repository
2. Install dependencies with `pnpm install`
3. Run the storybook or dev environment (if available)
4. Open a pull request

## 🛠 Environment Variables

No environment variables are required for this library.

## 📄 License

ISC

---

- [Repository](https://github.com/nikxpro/nikx-ui)
- [Issues](https://github.com/nikxpro/nikx-ui/issues)

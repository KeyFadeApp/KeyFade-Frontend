![KeyFade Logo](https://public.keyfade.com/logo.png)

**KeyFade** is a secure, link-based encryption tool that allows users to encrypt secrets into shareable links with a specified expiration period. This project includes a user-friendly front-end with Chakra UI, built on Vite, and connects to a secure backend API for encryption and storage of sensitive information.

---

## Features

- **Encrypted Link Generation**: Easily create secure, encrypted links for sensitive data.
- **Link Expiry Options**: Choose from various expiry durations for your encrypted links.
- **Responsive UI**: A clean and responsive interface, styled with Chakra UI and customized with Tailwind CSS.
- **Customizable Themes and Settings**: Modify colors, labels, and other UI properties using environment variables.

---

## Table of Contents

1. [Getting Started](#getting-started)
2. [Installation](#installation)
3. [Environment Variables](#environment-variables)
4. [How to Use](#how-to-use)
5. [Deployment](#deployment)
6. [Contributing](#contributing)
7. [License](#license)

---

## Getting Started

### Prerequisites

- **Node.js**: Ensure Node.js is installed on your machine.
- **npm**: This project uses `npm` for package management.

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/keyfade.git
   cd keyfade
   ```

2. Install dependencies:
   ```bash
   npm instalL
   ```

3. Set up environment variables by creating a .env file in the project root:
   ```bash
   cp .env.example .env
   ```

4. Start the development server:
   ```bash
   npm run dev
   ```

### Environment Variables

URLs & Secrets
```
VITE_LOGO_URL=https://public.keyfade.com/logo.png
VITE_FAVICON_URL=/favicon.ico
VITE_BACKEND_URL=https://demo-api.keyfade.com
VITE_FRONTEND_URL=https://demo.keyfade.com
VITE_HMAC_SECRET=<your_hmac_shared_secret>
```

Labels
```
VITE_CREATE_PASSWORD_LABEL=Secret to Encrypt:
VITE_CREATE_EXPIRY_OPTIONS_LABEL=Expiry Options:
VITE_LINK_GENERATED_LABEL=Encrypted Link:
VITE_LINK_COPY_LABEL=Copy Link
VITE_SECRET_LABEL=Secret:
```

UI Colors
```
VITE_EXPIRY_SLIDER_COLOR=purple
VITE_TEXT_COLOR=black
VITE_BUTTON_COLOR=purple
VITE_LINK_BUTTON_COLOR=purple
VITE_NOT_FOUND_BUTTON_COLOR=purple
VITE_DELETE_BUTTON_COLOR=#FED7D7
```

### How to use

- **1. Enter a Secret:** On the home page, enter the text you wish to encrypt.
- **2. Select Expiry:** Choose an expiry duration for the encrypted link.
- **3. Generate Link:** Click the "Generate Link" button to produce a secure, shareable link.
- **4. Copy and Share:** Use the "Copy Link" button to copy the generated link to your clipboard, and share it as needed.

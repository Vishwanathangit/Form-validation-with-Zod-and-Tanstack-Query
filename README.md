# 🧾 Form Validation with Zod and TanStack Query

A **multi-step, fully validated, and responsive registration form** built using **React**, **TypeScript**, **Zod**, **TanStack Query**, **React Hook Form**, and **Tailwind CSS**.

> 🌗 Includes a beautiful light/dark mode switcher and polished UI with validation feedback.

---

## 📁 Project Structure

```bash
├── public/
├── src/
│   ├── components/
│   │   ├── StepOne.tsx         # Step 1: Name & Email
│   │   ├── StepTwo.tsx         # Step 2: Personal Details (Gender, Age, etc.)
│   │   ├── StepThree.tsx       # Step 3: Address, Skills, About You
│   │   ├── Success.tsx         # Final Success screen after submission
│   │   └── ThemeToggle.tsx     # Light/Dark theme toggle button
│   ├── lib/
│   │   └── queryClien.tsx      # TanStack Query client instance
│   ├── App.tsx                 # Main form flow logic (3 steps + submission)
│   ├── main.tsx                # App root + QueryClientProvider
│   ├── types.ts                # Zod schema and form types
│   ├── index.css               # Tailwind CSS styles
│   └── vite-env.d.ts
├── index.html
├── tsconfig.json
├── tsconfig.app.json
├── tsconfig.node.json
├── vite.config.ts             # Vite + Tailwind plugin setup
└── eslint.config.js
```

---

## 🚀 Features

- ✅ Multi-step form navigation with "Next" and "Previous" buttons
- ✅ Field-level validations using **Zod**
- ✅ Smart form management using **React Hook Form**
- ✅ Optimized with **TanStack Query**
- ✅ Responsive design using **Tailwind CSS**
- ✅ Light/Dark mode support with persistence
- ✅ Summary of submitted data shown on final step
- ✅ TypeScript strictly enforced throughout

---

## 🧠 Technologies Used

| Technology         | Purpose                                    |
|--------------------|--------------------------------------------|
| React              | UI Library                                 |
| TypeScript         | Type safety and modern JavaScript features |
| React Hook Form    | Form state and integration                 |
| Zod                | Schema-based form validation               |
| TanStack Query     | Global client-side data state (QueryClient)|
| Tailwind CSS       | Utility-first CSS framework                |
| Vite               | Lightning fast dev environment             |

---

## 🧩 Form Flow

1. **Step 1 – Basic Info**: Name, Email  
2. **Step 2 – Personal Info**: Gender, Age, Phone, Hobbies, Country, Profession  
3. **Step 3 – Additional Info**: Address, City, ZIP, Education, Experience, Skills, About You  
4. **Submit**: Displays a clean summary and option to "Fill Another Form"

---

## 📦 Getting Started

### Prerequisites

- Node.js >= 16
- npm or yarn

### Installation

```bash
# Clone the repo
git clone https://github.com/your-username/form-validation-zod.git

# Navigate to project folder
cd form-validation-zod

# Install dependencies
npm install
```

### Development

```bash
npm run dev
```

### Build

```bash
npm run build
```

---

## 🌙 Dark Mode Support

Dark mode is auto-enabled based on system preferences, and users can toggle between light/dark modes via a floating button at the top-right.

---

## 🧪 Validation Highlights (Zod)

- Email format
- Indian phone number format (`+91 1234567890`)
- Age between 18 and 100
- ZIP code must be 6 digits
- "About You" must be at least 10 characters and not just spaces
- At least 1 skill and 1 hobby must be selected

Zod schema lives in `src/types.ts`.

---

## 🛠️ Custom Hooks / Utilities

- `queryClient` in `src/lib/queryClien.tsx` – a singleton instance of TanStack Query Client

---

## 💡 Best Practices

- All form state is type-safe using `FormData` from Zod inference
- Step-based validation ensures progressive checks
- Uses `trigger(fields)` from React Hook Form to validate current step
- Code is modular – each step is separated into its own component

---

## 📃 License

This project is licensed under the [MIT License](LICENSE).

---

## 💬 Feedback & Contributions

If you find a bug or want to contribute:
- Open an [Issue](https://github.com/your-username/form-validation-zod/issues)
- Create a [Pull Request](https://github.com/your-username/form-validation-zod/pulls)

---

## 🧠 Learn More

- [Zod Docs](https://zod.dev)
- [TanStack Query](https://tanstack.com/query/latest)
- [React Hook Form](https://react-hook-form.com/)
- [Tailwind CSS](https://tailwindcss.com/)

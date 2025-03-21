# DeepSeek AI Chat Application

A modern, responsive AI chat application built with Next.js and powered by DeepSeek's AI model. This application allows users to create, manage, and interact with AI through a sleek and intuitive interface.

## Features

- **AI Chat Interaction**: Engage with DeepSeek's powerful AI model through a chat interface
- **Chat Management**: Create, rename, delete, and organize your chat conversations
- **User Authentication**: Secure user authentication powered by Clerk
- **Responsive Design**: Fully responsive interface that works on desktop and mobile devices
- **Markdown Support**: AI responses support markdown formatting with code highlighting
- **Real-time Feedback**: Visual indicators for message loading states

## Technologies Used

### Frontend
- **Next.js 15**: React framework with App Router for efficient page rendering
- **React 19**: JavaScript library for building user interfaces
- **TailwindCSS 4**: Utility-first CSS framework for styling
- **React Markdown**: For rendering markdown in AI responses
- **Prism.js**: For syntax highlighting in code blocks
- **React Hot Toast**: For notification system

### Backend
- **Next.js API Routes**: Server-side API endpoints
- **MongoDB**: Database for storing chat history and user data
- **Mongoose**: MongoDB object modeling for Node.js
- **Clerk**: User authentication and management
- **DeepSeek API**: AI model integration for generating responses

## Project Structure

```
├── app/                 # Next.js App Router structure
│   ├── api/             # API routes for backend functionality
│   │   ├── chat/        # Chat-related API endpoints
│   │   └── clerk/       # Clerk webhook endpoints
│   ├── globals.css      # Global CSS styles
│   ├── layout.js        # Root layout component
│   └── page.jsx         # Main application page
├── assets/              # Static assets like icons and images
├── components/          # Reusable React components
├── config/              # Configuration files
├── context/             # React context for global state management
├── models/              # Mongoose data models
└── public/              # Public static files
```

## Getting Started

### Prerequisites
- Node.js (latest LTS version recommended)
- MongoDB instance
- DeepSeek API key
- Clerk account

### Installation

1. Clone the repository
   ```
   git clone https://github.com/yourusername/deepseek.git
   cd deepseek
   ```

2. Install dependencies
   ```
   npm install
   ```

3. Set up environment variables in a `.env.local` file
   ```
   DEEPSEEK_API_KEY=your_deepseek_api_key
   MONGODB_URI=your_mongodb_connection_string
   NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
   CLERK_SECRET_KEY=your_clerk_secret_key
   ```

4. Run the development server
   ```
   npm run dev
   ```

5. Open [http://localhost:3000](http://localhost:3000) in your browser

## Deployment

This application can be deployed on Vercel or any other Next.js-compatible hosting platform.

```
npm run build
npm start
```

## License

[MIT](https://choosealicense.com/licenses/mit/)
# Bright Path 🚀

### An AI-Powered Learning Co-Pilot for the Next Generation

Bright Path isn't just another task manager. It's a personal learning platform born from a real-life problem: how can a busy parent (or older sibling!) guide a child's education in an age of digital distractions? This project was built to turn passive screen time into active, confidence-boosting skill-building.

thsi is the youtub demo : https://youtu.be/_nvFy1KwZZc?si=RA73AVpLTvQp951L

---
<img width="595" height="389" alt="لقطة شاشة 2025-04-02 211114" src="https://github.com/user-attachments/assets/3f977cae-b9e5-4c63-a794-b15a3e9381ae" />


## The Story Behind Bright Path

The inspiration for this project is my 10-year-old brother. I always wanted to teach him tech skills, but our opposite school schedules made it impossible. I'd leave him my laptop to learn, but I'd come back to find him watching YouTube or playing games.

I built Bright Path to be the bridge. Now, I can set a learning "mission" for him in the morning, and a powerful AI tutor guides him through it, step-by-step. At the end of the day, we can talk about what he actually accomplished.

## ✨ Core Features

### For Parents & Guardians
*   👨‍👩‍👧 **Personalized Task Creation:** Set learning goals on any topic, from coding to history.
*   🧠 **AI-Generated Learning Plans:** Our AI (powered by Gemini 1.5 Pro) automatically creates engaging, step-by-step learning paths tailored to your child.
*   📊 **Real-Time Progress Tracking:** See what your child has accomplished throughout the day.
*   🏆 **Customizable Rewards:** Motivate your child by setting up a fun and rewarding points system.

### For Kids
*   🎮 **Gamified "Mission" Interface:** Kids see a fun and simple dashboard with their "missions" for the day.
*   🤖 **The Context-Aware AI Tutor:** This is our magic feature! When a child gets stuck, our AI assistant (powered by ScreenPipe) **sees their screen**, understands the exact problem, and provides helpful, real-time guidance. No more generic chatbot answers!

## 🛠️ Technology Stack

*   **Frontend:** React.js, Material-UI
*   **Backend & Auth:** Supabase
*   **AI Planner:** Google Gemini 1.5 Pro
*   **Context-Aware AI Tutor:** [**ScreenPipe**](https://github.com/emil-ernerfeldt/screenpipe) - The core technology that gives our AI "eyes" to see the user's screen.

## 🚀 Getting Started: How to Run Bright Path

This project has two main components: the **Bright Path web application** and the **ScreenPipe** local server that powers the AI assistant. You must have both running.

### Prerequisites
*   Node.js and npm/yarn
*   Git

### Step 1: Install and Run ScreenPipe (The AI "Eyes")

> **IMPORTANT:** Bright Path's context-aware AI Tutor **will not work** without ScreenPipe running locally on your machine.

1.  **Download ScreenPipe:** Go to the official [ScreenPipe GitHub Releases page](https://github.com/emil-ernerfeldt/screenpipe/releases) and download the appropriate version for your operating system (Windows, macOS, Linux).
2.  **Install & Run:** Follow the installation instructions provided by ScreenPipe. Once installed, launch the application. You should see a terminal or console window indicating that the ScreenPipe server is running.
3.  Keep this running in the background.

### Step 2: Clone and Set Up the Bright Path App

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/ayoub0030/parentale-assistante.git
    cd parentale-assistante
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

### Step 3: Configure Environment Variables

1.  Create a `.env.local` file in the root of the project.
2.  Add your credentials for Supabase and Google Gemini. It should look like this:

    ```env
    # .env.local.example

# Gemini API Configuration
GEMINI_API_KEY=your_gemini_api_key_here

# Next.js Configuration
NEXTAUTH_URL=http://localhost:3000
NEXTAUTH_SECRET=your_nextauth_secret_here

# Application Configuration
NODE_ENV=development

# Supabase Configuration
NEXT_PUBLIC_SUPABASE_URL=https://your-project-id.supabase.co
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key_here

    ```

### Step 4: Run the Application

1.  Make sure your ScreenPipe server from Step 1 is still running.
2.  Start the development server for Bright Path:
    ```bash
    npm run dev
    ```
3.  Open your browser and navigate to `http://localhost:3000`. You should now be able to use the application!

## 🖼️ Screenshots

_Update these with your new screenshots if needed_

![Child Profiles](<link-to-your-screenshot-1.png>)
_Parental view to manage child profiles and tasks._

![AI Chat Assistant](<link-to-your-screenshot-2.png>)
_The context-aware AI assistant helping a child with a Python task._


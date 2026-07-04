# Virtual Stock Exchange Platform (VSE) 
A real-time Virtual Stock Exchange platform developed for the 20th NYCU IMF Camp. This system provides participants with an immersive, competitive, and technically robust environment to simulate real-market trading.

**URL** <br>[https://imfvse.vercel.app/]
## 💡Features
### Real-time Market Simulation
- Leverages Firebase Firestore to achieve millisecond-level data synchronization, ensuring all participants experience price fluctuations in perfect unison.
- mplements stochastic price movement algorithms to replicate real-world market volatility, adding unpredictability and excitement to trading sessions.
- Highly optimized frontend architecture to ensure the environment remains responsive even during high-volume trading bursts.
### Advanced Trading Mechanisms
- Supports flexible market orders, including both Long (Buy) and Short-selling (Sell) positions, enabling diverse investment strategies.
- Handles complex calculations in real-time, including:
  
  - Automated margin call detection for bankrupt positions.
  - Dynamic interest rate and borrowing cost accruals.
  - Real-time buying power calculation based on portfolio valuation and debt levels.
- Integrated transaction cost algorithms to simulate brokerage fees, borrowing costs, and market slippage, forcing participants to account for expenses.
### Dynamic Leaderboard & Analytics
- Automatically computes total asset value and Return on Investment (ROI) across all teams in real-time.
- Visualizes competitive standings with trend indicators, allowing teams to instantly gauge their position relative to peers.
### Admin & Oversight System
-  Dedicated administrative dashboard to toggle market status (Open/Close) for specific trading sessions.
-  A notification engine capable of pushing simulated news updates to all participants instantly.
- Capabilities for admin to adjust:
  
  - Inflation system
  - Service/Lending Fee
  - Manual Cash Adjust
  - New Stock info
###  Responsive UX Design (RWD)
- Interface crafted for rapid interaction on participants' smartphones, ensuring ease of use during high-pressure trading sessions.
- Tested across desktop, tablet, and mobile browsers.
## 🛠️ Tech Stack
- Frontend: React.js + Vite
- Backend & Database: Firebase Firestore (Realtime Data Streaming)
- Authentication: Firebase Authentication (Anonymous Session Management)
- Styling: Tailwind CSS
- Deployment: Vercel
## Local Setup
### Prerequisites
- Node.js 
- npm
### Steps
1. Clone the repository
```bash
git clone https://github.com/Hu4y/VSE.git
cd VSE
```

2. Install dependencies
```bash
npm install
```
3. Set up environment variables
```bash
cp .env.example .env
```
Fill in your credentials in `.env` (Firebase)

4. Run the development server
```bash
npm run dev
```

Open http://localhost:5173 in your browser.

## How to Use
### For Teams
1. Login: Navigate to the home page, select your designated team from the dropdown, and enter the secret PIN assigned to your team.
2. Trade: Use the "Market" tab to view live stock charts and place Buy/Sell orders.
3. Monitor: Use the "Portfolio" tab to track your current holdings, average costs, and total Return on Investment (ROI).
### For Admins
1. Access Panel: Click the secret shield icon on the login screen to access the Admin Console.
2. Market Management: Use the control center to toggle the market status between "Open" and "Closed."
3. Round Progression: Use the "Advance to Round" button to finalize pricing and apply interest fees at the end of each session.
4. Broadcast: Use the "News Feed" input to send urgent announcements to all team terminals.
5. Monitor: Access the "Team Monitor" panel to track real-time asset values, buying power, and individual team trade logs.
## ⚠️ Security Notice
- Ensure .env is included in your .gitignore file.
- When deploying to Vercel, inject your keys via the Environment Variables dashboard in the Vercel settings.
---
This system is developed exclusively for educational purposes for the 20th NYCU IMF Camp. The trading simulations, market data, and financial outcomes generated within this platform are for instructional use only and do not reflect real-world financial advice or market performance.

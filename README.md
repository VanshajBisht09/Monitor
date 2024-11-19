🧰 Setup Instructions
Prerequisites
React
Go
Redis
Backend Setup
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/exploding-kitten.git
cd exploding-kitten
Navigate to the backend directory:

bash
Copy code
cd backend
Install dependencies:

bash
Copy code
go mod tidy
Run the server:

bash
Copy code
go run main.go
Frontend Setup
Navigate to the frontend directory:

bash
Copy code
cd frontend
Install dependencies:

bash
Copy code
npm install
Start the development server:

bash
Copy code
npm start
Redis Setup
Start the Redis server:

bash
Copy code
redis-server
Configure the backend to connect to Redis (update config.yaml or .env with Redis host and port if necessary).



This will be an online single-player card game that consists of 4 different types of cards

- Cat card 😼
- Defuse card 🙅‍♂️
- Shuffle card 🔀
- Exploding kitten card 💣

There will be a button to start the game. When the game is started there will be a deck of 5 cards ordered randomly. Each time user clicks on the deck a card is revealed and that card is removed from the deck. A player wins the game once he draws all 5 cards from the deck and there is no card left to draw.

Rules –
- If the card drawn from the deck is a cat card, then the card is removed from the deck.
- If the card is exploding kitten (bomb) then the player loses the game.
- If the card is a defusing card, then the card is removed from the deck. This card can be used to defuse one bomb that may come in subsequent cards drawn from the deck.
- If the card is a shuffle card, then the game is restarted and the deck is filled with 5 cards again.

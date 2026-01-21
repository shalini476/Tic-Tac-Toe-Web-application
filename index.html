<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tic-Tac-Toe</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
        }
        .board {
            display: grid;
            grid-template-columns: repeat(3, 100px);
            grid-template-rows: repeat(3, 100px);
            gap: 5px;
            justify-content: center;
            margin-top: 20px;
        }
        .cell {
            width: 100px;
            height: 100px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2em;
            background-color: lightgray;
            cursor: pointer;
        }
        .cell.taken {
            pointer-events: none;
        }
    </style>
</head>
<body>
    <h1>Tic-Tac-Toe</h1>
    <div class="board" id="board"></div>
    <h2 id="status">Player X's turn</h2>
    <button onclick="resetGame()">Restart Game</button>

    <script>
        const board = document.getElementById("board");
        const status = document.getElementById("status");
        let currentPlayer = "X";
        let gameState = ["", "", "", "", "", "", "", "", ""];

        function createBoard() {
            board.innerHTML = "";
            gameState.forEach((cell, index) => {
                const cellElement = document.createElement("div");
                cellElement.classList.add("cell");
                cellElement.dataset.index = index;
                cellElement.textContent = cell;
                cellElement.addEventListener("click", handleMove);
                board.appendChild(cellElement);
            });
        }

        function handleMove(event) {
            const index = event.target.dataset.index;
            if (gameState[index] === "" && currentPlayer === "X") {
                gameState[index] = currentPlayer;
                event.target.textContent = currentPlayer;
                event.target.classList.add("taken");
                if (checkWinner()) {
                    status.textContent = Player ${currentPlayer} wins!;
                    disableBoard();
                    return;
                }
                if (!gameState.includes("")) {
                    status.textContent = "It's a draw!";
                    return;
                }
                currentPlayer = "O";
                status.textContent = "AI's turn";
                setTimeout(aiMove, 500);
            }
        }

        function aiMove() {
            let availableMoves = gameState.map((cell, index) => cell === "" ? index : null).filter(index => index !== null);
            if (availableMoves.length > 0) {
                let bestMove = getBestMove();
                gameState[bestMove] = "O";
                document.querySelector([data-index='${bestMove}']).textContent = "O";
                document.querySelector([data-index='${bestMove}']).classList.add("taken");
                if (checkWinner()) {
                    status.textContent = "AI wins!";
                    disableBoard();
                    return;
                }
                if (!gameState.includes("")) {
                    status.textContent = "It's a draw!";
                    return;
                }
                currentPlayer = "X";
                status.textContent = "Player X's turn";
            }
        }

        function getBestMove() {
            let availableMoves = gameState.map((cell, index) => cell === "" ? index : null).filter(index => index !== null);
            return availableMoves[Math.floor(Math.random() * availableMoves.length)];
        }

        function checkWinner() {
            const winningCombinations = [
                [0, 1, 2], [3, 4, 5], [6, 7, 8], 
                [0, 3, 6], [1, 4, 7], [2, 5, 8], 
                [0, 4, 8], [2, 4, 6]
            ];
            return winningCombinations.some(combination => {
                const [a, b, c] = combination;
                return gameState[a] && gameState[a] === gameState[b] && gameState[a] === gameState[c];
            });
        }

        function disableBoard() {
            document.querySelectorAll(".cell").forEach(cell => cell.removeEventListener("click", handleMove));
        }

        function resetGame() {
            gameState = ["", "", "", "", "", "", "", "", ""];
            currentPlayer = "X";
            status.textContent = "Player X's turn";
            createBoard();
        }

        createBoard();
    </script>
</body>
</html>

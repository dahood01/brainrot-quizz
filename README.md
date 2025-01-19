# brainrot-quizz
<html>
    <head>
        <title>
            BRAINROT QUIZZZ 
        </title>
    </head>
    <body>
        <script>

            // define the function
            function showMessage() {
            alert("Hello! Welcome to the brainrot Quizzz.");
            }
             // call this function 
             showMessage();
                </script>
            
            <script>

                // define the function
                function showMessage() {
                alert("We will begin the ultimate brainrot quizzz.");
                }
                // call this function 
                showMessage();
                </script>
                
                <script>
                // define the function
                function showMessage() {
                alert("If you get any question wrong ill come to your home lil bro.");
                }
                // call this function 
                showMessage();
                </script>
                <h2> LEVEL OF DIFFICULTY= easy peasy lemon squeezy <h2>
                    <br>
                    <img src="Shrek.jpeg"  
                    alt="sus guy" 
                    title="weird bald guy?!">

                    
                    <!-- Question 1 -->
                    <form id="quizForm">
        <p>1. who is this guy?</p>
        <input type="radio" name="q1" value="shrek"> shrek<br>

        <input type="radio" name="q1" value="ksi"> ksi<br>

        <input type="radio" name="q1" value="good boy"> good boy<br>

        <input type="radio" name="q1" value="skibidi toilet"> skibidi toilet<br>
         
        <img src="mewing 🤫🧏.jpeg">

        <!-- Question 2 -->
        <p>2. What is this? </p>
        <input type="radio" name="q2" value="weird face"> weird face<br>

        <input type="radio" name="q2" value="sigma boy"> sigma boy<br>

        <input type="radio" name="q2" value="mewing"> mewing<br>

        <input type="radio" name="q2" value="idk"> idk<br>

<img src="f4bc810d-5b96-4644-95a7-40935d1ef701.jpeg">

    <!-- Question 3 -->
     <p>3. what is he doing? </p>
     <input type="radio" name="q3" value="he is rizzing"> he is rizzing<br>

     <input type="radio" name="q3" value="idk"> idk<br>

     <input type="radio" name="q3" value="he is talking with friends"> he is talking with friends<br>

     <input type="radio" name="q3" value="none of the above"> none of the above<br>

        <!-- Submit Button -->
        <button type="button" onclick="showResults()">Submit</button>
    </form>

    <h2>Results</h2>
    <p id="results"></p>

    <script>
        function showResults() {
            // Correct answers
            const correctAnswers = {
                q1: "shrek",
                q2: "mewing",
                q3: "he is rizzing"
            };


            // User answers
            const userAnswers = new FormData(document.getElementById("quizForm"));
            let score = 0;
            let resultText = "";

            // Check answers
            for (const [question, answer] of userAnswers.entries()) {
                if (answer === correctAnswers[question]) {
                    score++;
                    resultText += `Question ${question.slice(1)}: Correct! 🎉<br>`;
                } else {
                    resultText += `Question ${question.slice(1)}: Wrong! The correct answer is ${correctAnswers[question]}.<br>`;
                }
            }

            // Display results
            const resultsElement = document.getElementById("results");
            resultsElement.innerHTML = `You scored ${score} out of ${Object.keys(correctAnswers).length}.<br><br>` + resultText;
        }
    </script>
                    
                
                </body> 
    </html>


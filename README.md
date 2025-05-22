# Aman Kumar – Developer of a Calculator Project

<h1>Hi I am Aman Kumar, a passionate and skilled web developer, has successfully designed and developed a dynamic calculator project using HTML and CSS. With a keen eye for clean design and user-friendly functionality, I am crafted this project as a testament to his dedication to front-end development. My journey was supported by the esteemed Study Comrad Institute, where he honed his skills and transformed his ideas into reality.</h1>

<img src = "https://github.com/Amansinha110/Calculator/blob/main/Screenshot%202025-05-22%20092825.png"> 

<h1>Example Code:-</h1>

<body>
    <div class="calculator">
        <div class="display">0</div>
        <div class="buttons">
            <button class="clear" onclick="clearDisplay()">C</button>
            <button class="operator" onclick="appendToDisplay('±')">±</button>
            <button class="operator" onclick="appendToDisplay('%')">%</button>
            <button class="operator" onclick="appendToDisplay('/')">÷</button>
            
            <button class="number" onclick="appendToDisplay('7')">7</button>
            <button class="number" onclick="appendToDisplay('8')">8</button>
            <button class="number" onclick="appendToDisplay('9')">9</button>
            <button class="operator" onclick="appendToDisplay('*')">×</button>
            
            <button class="number" onclick="appendToDisplay('4')">4</button>
            <button class="number" onclick="appendToDisplay('5')">5</button>
            <button class="number" onclick="appendToDisplay('6')">6</button>
            <button class="operator" onclick="appendToDisplay('-')">-</button>
            
            <button class="number" onclick="appendToDisplay('1')">1</button>
            <button class="number" onclick="appendToDisplay('2')">2</button>
            <button class="number" onclick="appendToDisplay('3')">3</button>
            <button class="operator" onclick="appendToDisplay('+')">+</button>
            
            <button class="number span-2" onclick="appendToDisplay('0')">0</button>
            <button class="number" onclick="appendToDisplay('.')">.</button>
            <button class="equals" onclick="calculate()">=</button>
        </div>
    </div>

    <script>
        let display = document.querySelector('.display');
        
        function appendToDisplay(value) {
            if(display.textContent === '0' && value !== '.') {
                display.textContent = value;
            } else {
                display.textContent += value;
            }
        }

        function clearDisplay() {
            display.textContent = '0';
        }

        function calculate() {
            try {
                let expression = display.textContent
                    .replace(/×/g, '*')
                    .replace(/÷/g, '/')
                    .replace(/±/g, '-');
                
                let result = eval(expression);
                display.textContent = result;
            } catch(error) {
                display.textContent = 'Error';
            }
        }
    </script>
</body>

<h1>The calculator project, although simple in concept, showcases clear design, responsiveness, and user-friendly interaction, making it a valuable demonstration of My skills in web technologies. By focusing on structured design and clean aesthetics, he has created an intuitive tool that provides essential arithmetic operations, giving users a seamless experience.</h1>

<h1>Aman Kumar's Journey in Web Development
From the beginning, Aman Kumar was fascinated with how websites are structured and how different components interact to form a well-functioning digital platform. His journey into coding started with learning the fundamental concepts of HTML, CSS, and JavaScript. As he progressed in his studies, he explored ways to create dynamic websites that are both visually appealing and highly functional.

Guided by Study Comrad Institute, Aman strengthened his coding abilities by working on small projects and gradually building expertise in web development. Recognizing that every great developer needs hands-on experience, he decided to create a calculator project, a tool that combines both visual design and logical structure.</h1>

<img src = "https://github.com/Amansinha110/Calculator/blob/main/Screenshot%202025-05-22%20092813.png">

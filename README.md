Fly Me to My Destination
Description
This project implements a solution to the "Fly Me to My Destination" problem using a greedy algorithm in JavaScript. The goal is to determine the minimum number of planes needed to travel from the first to the last airport, given an array where each element represents the fuel units available at each airport.

Problem Statement
Given N airports, each with a plane having a certain number of fuel units available, you need to travel from the first airport to the last airport by hiring the minimum number of planes. One unit of fuel is needed to fly to the next nearest airport.

Example
Input: [2, 1, 2, 3, 1]

Output: 2

Input: [1, 6, 3, 4, 5, 0, 0, 0, 6]

Output: 3

Algorithm
Greedy Algorithm
A greedy algorithm is used to solve this problem efficiently. The main idea is to always choose the plane that can take you the farthest from your current position.

Steps
Initialization: Start from the first airport.
Track Reach: Keep track of the farthest airport that can be reached.
Hire New Plane: Whenever the current plane's limit is reached, hire a new plane that extends the reach.
Check Completion: If the last airport is reachable, return the plane count; otherwise, return -1.
Why Greedy Algorithm?
The greedy algorithm is suitable for this problem because it allows making local optimal choices at each step to achieve a global optimum. By always choosing the plane that extends the maximum reach, we ensure that the minimum number of planes is used to reach the destination.

Project Structure
index.html: The main HTML file containing the form for user input and the script inclusion.
main.js: JavaScript file implementing the algorithm and handling user inputs.
Usage
Clone the repository:
bash
Copy code
git clone https://github.com/your-username/fly-me-to-my-destination.git
Navigate to the project directory and open index.html in a web browser.
Enter a comma-separated list of fuel units in the input field and click the "Calculate" button.
The result will be displayed on the page.
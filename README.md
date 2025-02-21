# Todo-List
Todo List Application


 **Approach Used in the To-Do List App**  
1. **Component Structure:**  
   - Created a single React component `TodoApp` to manage the entire application.  
   - Used **functional components** and **React hooks** (`useState`) for state management.  

2. **State Management:**  
   - Used `useState` to maintain the list of tasks and track user input.  
   - Each task is an object with `{ text, completed }`, allowing for easy toggling of completion status.  

3. **Event Handling:**  
   - `addTask()`: Adds a new task if input is not empty.  
   - `deleteTask()`: Removes a task based on its index.  
   - `toggleTaskCompletion()`: Updates a task’s `completed` status when clicked.  

4. **UI & Styling:**  
   - Used **Tailwind CSS** for styling, ensuring a clean and responsive design.  
   - Input field and button allow users to add tasks conveniently.  
   - Tasks are displayed in a list with options to **mark as completed** (via strikethrough effect) and **delete** them.  

---

 **Challenges Faced & Solutions**
1. **Managing State Updates Properly:**  
   - Initially, tasks were getting modified incorrectly. Solved by using **immutable updates** (`setTasks([...tasks, newTask])` instead of directly mutating state).  

2. **Handling UI Responsiveness:**  
   - Needed proper spacing and alignment, which was handled efficiently with Tailwind CSS.  

3. **Ensuring Accessibility and UX:**  
   - Added **click events** to toggle task completion for a better user experience.  
   - Prevented adding empty tasks to keep the list meaningful.  


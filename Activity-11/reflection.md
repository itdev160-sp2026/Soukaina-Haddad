# Activity 11 Reflection: React Tic-Tac-Toe

### Key Learnings

* **Components**
Breaking the UI into smaller, bite-sized pieces made the whole project feel way less overwhelming. I learned that each component should really only have one job, and once you have those pieces, you just piece them together like Legos to build the full app.
* **useState (State Management)**
This is what keeps track of all the data. The coolest part is that when the state changes, React just handles the screen updates for me. I didn't have to go in and manually mess with the DOM like I did in the last project.
* **Props (Passing Data)**
I used these to send info from the parent components down to the children. It’s basically like passing parameters into a function, and it keeps the data flow feeling really organized and easy to follow.
* **Immutability**
I learned why it's important to use `.slice()` to make copies of arrays instead of just editing them directly. It felt like an extra step at first, but it’s actually how React knows exactly what changed, and it’s the only reason features like the move history actually work.

---

### Comparison with Activity 10 (Vanilla JS vs React)

* **State Updates:** In Vanilla JS, I had to manually update the DOM every time something changed. In React, it just happens automatically whenever the state is updated.
* **Code Organization:** My Vanilla JS code was kind of all over the place, but React forced me to keep everything organized into specific components.
* **Adding Features:** Trying to add new logic in Vanilla JS felt like I might break the whole thing, but React's structure made adding new stuff way more manageable.
* **Reusability:** Vanilla JS felt like a one-off, but React components are super easy to reuse in different parts of the app.
* **Learning Curve:** Vanilla JS was definitely easier to get started with, but React feels way more powerful once you get past the initial hurdle.
* **Data Flow:** My data got pretty messy in Vanilla JS, while React keeps a very clear, one-way flow using props.
* **History / Time Travel Feature:** This would have been a nightmare to code in Vanilla JS, but it’s basically built into the way React handles state.
* **UI Updates:** I had to track every single change myself in Vanilla JS, whereas React handles the heavy lifting for the UI.

---

### Challenges

* **State Lifting:** It took me a minute to realize why the state had to live in the `Game` component rather than the `Board`. I eventually understood that it was the only way to share that data across the different pieces of the UI.
* **Immutability:** I was definitely confused about why I couldn't just edit arrays directly. It makes way more sense now that I see how it triggers React's update process.
* **JSX:** Mixing HTML-looking code with JavaScript felt really weird at first. I kept forgetting to use `className` instead of `class`, and it took some practice to know exactly when I needed to wrap things in curly braces `{}`.

---

### What Worked Well

The time travel feature was surprisingly easy to implement once I understood how state worked. Using components definitely made my code look a lot cleaner than my previous projects, and once `useState` finally clicked, everything else started falling into place.

---

### Next Steps

* Get a handle on **`useEffect`** for side effects.
* Learn how to build **custom hooks**.
* Look into **React Router** for multi-page apps.
* Check out state management tools like **Redux** or **Zustand**.
* Start using **Vite** instead of older setup tools.
* Work on finding even better ways to structure my components.

---

### Conclusion

React definitely makes building apps more efficient compared to Vanilla JS. Even though it's harder to learn at first, the way it handles updates and organization is a total game-changer. It’s definitely worth the effort once you start to see how it all fits together.
# **🎬 Case Study: The Netflix Data Engine**

## **The Scenario**

Netflix doesn't just show you movies; it predicts what you want before you know it. This recommendation system is a perfect example of the **Data Lifecycle**.

## **👥 Group Discussion Questions**

Break into small groups and answer the following. Use your knowledge of Structured vs. Unstructured data.

### **Part 1: Collection (What data do they have?)**

*List at least 3 examples for each category that Netflix likely collects about you:*

* **Explicit Data (Information you intentionally provide):** (e.g., Typing a search query, filling out your profile, giving a Thumbs up/down...)

> 1. Ratings: Clicking "Thumbs Up," "Double Thumbs Up," or "Thumbs Down" on a movie or drama.
> 2. Search Queries: Selecting maturity ratings, primary language/subtitle preferences.
> 3. Profile setup: Typing specific film or drama titles or actor names

* **Implicit Data (Behaviors observed in the background):** (e.g., Did you pause at a scary scene? Did you binge-watch 5 episodes? How fast did you scroll?)

> 1. Viewing patterns: Logging exactly when I watch (time of day, day of week) and my streaming duration in a single session.
> 2. Playback Actions: Pausing, rewinding, fast-forwarding, skipping intro credits, or abandoning a show halfway through.
> 3. Browsing Behavior: Hovering over a tile, scrolling past a row without clicking, or time spent looking at a preview drama or film before hitting play.

---

### **Part 2: Structured vs. Unstructured**

* **Structured Data:** User ID, Movie Genre, Release Year.  
* **Unstructured Data:** The movie thumbnails (images), the movie plot summary (text), the video files themselves.  
  * *Question: How might Netflix use the **Unstructured** data (thumbnails) to trick you into watching a movie?*

  > A user who watches a lot of dark crime thrillers might see a dark, shadowy, high-contrast thumbnail for a drama. On the other hand, a user who prefers mainstream action blockbusters might see a different thumbnail for the exact same film featuring an explosion, a car chase, or an intense fight scene.

---

### **Part 3: The Algorithm (Analysis)**

* If User A watches "Breaking Bad" and "Better Call Saul".  
* And User B watches "Breaking Bad".  
* *What will the algorithm recommend to User B? Why?*

> It will suggest "Better Call Saul". The algorithm looks across millions of users to find patterns in what content is watched together. It detects that users who watch Breaking Bad have a very high probability of also watching Better Call Saul. Since User A moved on to "Better Call Saul" after "Breaking Bad", the system predicts that User B — having the same foundational interest — may also watch "Better Call Saul".

---

### **Part 4: Ethics (The "Bubble")**

* *Is it ethical for an algorithm to only show you things it knows you will like? Does this create a 'content bubble' that limits your exposure to new ideas?*

> Ethics depend on the type of content being filtered and the intent behind the system. For Netflix, content personalisation is generally seen as benign or even beneficial. Recommendation systems save users' time, improve convenience, and help users find entertainment that they actually enjoy out of millions of choices. However, over-indexing on past behavior can trap users in a comfort zone — preventing them from discovering new contents or genres which they may have loved if given the chance.

---

<details>
<summary>💡 Discussion pointers (open after you've tried)</summary>

**Part 1: Collection**

- **Explicit Data (intentionally provided info):** Thumbs up/down ratings, adding a show to "My List", the search terms you type, the profile/maturity settings you choose.
- **Implicit Data (things you do):** How long you watch before quitting, whether you binge 5 episodes in one night, what time of day you watch, whether you rewind or pause at certain scenes, which thumbnail finally made you click after scrolling past three times.


**Part 2: Structured vs. Unstructured — the thumbnail trick**

Netflix analyses its unstructured images to learn which *kind* of artwork makes *you* click. If you tend to watch romances, the same movie might be shown to you with a thumbnail of the couple; if you watch action, you'd see the explosion scene instead. Different users see different artwork for the same title — the unstructured data (images) is being mined to personalise the "packaging."

**Part 3: The Algorithm**

The algorithm will likely recommend **"Better Call Saul" to User B**. Why? Because User A and User B overlap (both watched "Breaking Bad"), so the system assumes their tastes are similar. This approach is called **collaborative filtering** — in plain English: *people who liked what you liked will probably like the same next thing — like asking a friend with similar taste for a movie tip*. The algorithm doesn't need to understand the shows at all; it just matches patterns of similar viewers.

**Part 4: Ethics — the "Bubble"**

There's no single right answer — good discussions usually surface both sides:

- *For:* Recommendations save time, reduce choice overload, and genuinely help people find things they enjoy.
- *Against:* If you're only ever shown what you already like, you're in a "content bubble" — your tastes narrow, new genres and viewpoints never reach you, and the platform's goal (keep you watching) may not match your goal (discover something meaningful). A strong answer also mentions possible fixes: injecting deliberate variety, "explore something new" rows, or giving users transparency and control over their recommendations.

</details>


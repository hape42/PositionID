# **The Core Idea**

Whenever I watched others play Backgammon, I wanted to remember certain positions to analyze them later with GNU BG (and later BGBlitz). Especially when I would have played a different move or chosen **take** instead of **pass**.

I used to carry a **paper notebook** with a pre-drawn board, but quickly noting a position was stressful since the game wouldn't wait for me.  
On top of that, manually entering these positions into GNU BG was tedious before I could finally analyze them and understand why the player didn't choose my move.

**Many years later, technology now offers ways to solve this problem in a much more efficient way.**

## **A Better Solution Than Frantic Writing?**

- I simply take a **photo** of the board (or a **screenshot**).  
- A **tool** analyzes the image and recognizes the Backgammon position.  
- It asks for missing or unclear information, such as:  
  - **Money game or match play?**  
  - **Current match score?**  
  - **Where is the cube? What level?**  
  - **Is the home board on the left or right?**  
  - **If checkers are missing, are they played out or on the bar?**  
- Once everything is clear, the tool converts the detected position into a **XGID/GNU ID**.

This **ID** can then be used in **BGBlitz, GNU BG, or XG Gammon** for further analysis.

---

## **First Technical Draft**

- The tool should run **locally** on all major platforms (**Mac, Windows, Linux, iOS, Android**).  
- I don’t want to reinvent the wheel from the start—so I’ll build upon existing tools where possible.  
- Image recognition will be done using **OpenCV**, later replaced by a **custom-trained AI model**.  
- The **frontend** is still undecided.  
- Since I currently have **zero** experience in these areas, I’ll start by taking a **Python course**.  
- All documents (including temporary drafts) will be stored on **GitHub**.  
- I will document **progress, challenges, and setbacks** in the form of a **project journal**.

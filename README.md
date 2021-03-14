# AutoPromPicker
Remember Prom Night? 🎶

One of the major issues ⚔ we faced was to ensure that all the handsome boys🤵 were paired to all the gorgeous girls💃 in a way that took care of everyone's priority 💛 and they don't break up for the night.

"Nah! That's just a fairytale scenario". Well I agree but python 🐍can help out to a great extent. 


As any other wizard🧙‍♂️ , python requires you to follow some rules ❗for this spell to work:

- The number of boys and girls must be equal. We don't want anyone to be left out in the corner. 💔
- Everyone should be brutually honest when asked about ranking their counterparts in order of preferrence.
- The guys get to propose the girls ( We can flip this if required)

# Some Theorical Background: 🔍

Our situation is an application of the popular [Stable Marriage Problem](https://en.wikipedia.org/wiki/Stable_marriage_problem). It can be solved by the[Gayle-Shapely algorithm](https://en.wikipedia.org/wiki/Gale%E2%80%93Shapley_algorithm) given below:

``` 
Initialize all m ∈ M and w ∈ W to free
    while ∃ free man m who still has a woman w to propose to do
        w := first woman on m's list to whom m has not yet proposed
        if w is free then
            (m, w) become engaged
        else some pair (m', w) already exists
            if w prefers m to m' then
                m' becomes free
                (m, w) become engaged 
            else
                (m', w) remain engaged
            end if
        end if
    repeat
   ```

# Usage:

Convinced..huh? 😉 and want this spell for yourself?

![usage](https://media.giphy.com/media/H2SiDhuGVJRWU/giphy.gif)

Here you go:

- clone or Download this repo ⏬
- Open the Terminal 🐱‍💻
- Move inside 👉 the repo 
```cd AutoPromPicker``` 
- Open ```autoprompick.py``` and change the names of the girls,boys and preferences as desired🧱 
- Now, the climax you have been waiting for!😎. Run the script using Terminal
  ```python autoprompick.py```
- Abracadabra ⚡

**I assume you have python installed on your system and set to path.**

# Further Work: 🏗
- Tune this script to take in the number of girls and boys from the terminal,their names and preference of each
- Create a GUI for this
- Deploy🚢 the above using Streamlit
- Create an end to end auto prom picker system, where the ```N``` boys and ```N``` girls register themselves,put up their profile,rate each other and our script takes those values and gives them their best pair(s) as per precedence of ask out 

# License 📜

[MIT License](https://github.com/smaranjitghose/AutoPromPicker/blob/master/LICENSE)

# **Crafted with ❤ by Smaranjit Ghose**

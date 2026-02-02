# Final Year Project
## Sign & Spell VR: ISL Alphabet Practice and Sentence Construction in VR

**What is the Project idea?**  

Sign & Spell VR is a virtual reality application that helps users learn Irish Sign Language (ISL) in an interactive way using the Meta Quest 3/3S and Godot 4. The system tracks the user’s hands in real time and focuses on teaching the ISL alphabet first, then simple words and everyday words, and finally a test-style mode to check what they remember.
 
**Why is it useful/unique?**  

Sign & Spell VR is a virtual reality application that helps users learn Irish Sign Language (ISL) in an interactive way using the Meta Quest 3/3S and Godot 4. The system tracks the user’s hands in real time and focuses on teaching the ISL alphabet first, then simple words and everyday words, and finally a test-style mode to check what they remember.

**What does it offer (e.g., To the User)?**  

Users can practice ISL letters and basic words in a 3D environment where their hand shapes are checked against stored ISL templates. The app gives simple on‑screen feedback and progress tracking so they know which signs they got right and which ones they need to fix before moving on to short sentences and quizzes 
 
**How will it Operate?**  

The app uses the Meta Quest 3/3S hand tracking, with Godot 4 and OpenXR handling the VR setup and controller-free interaction. A rule-based system compares detected hand poses to predefined ISL letter shapes saved in data files, then updates the VR UI to show results and store basic progress for later sessions.
 
**Why is this a good idea and what will the end deliverable be?**  

There are very few interactive tools for learning ISL, especially in VR, so this project helps fill that gap while still being simple enough to run as a prototype. The end deliverable is a working VR prototype that demonstrates alphabet practice, basic spelling, and feedback, and it also sets up a clear path to extend the system with more signs, better recognition, and extra learning modes in the future.

## Weekly Logs
### Week 5 - Expanding My Research
This week I mainly focused on my research and tried to strengthen my literature review. I spent most of the time reading about different sign language apps and how VR is being used for learning. I realised there’s not much out there for Irish Sign Language (ISL), so most of what I found was about American Sign Language (ASL).

I looked into apps like ASL Fingerspeller, Silent Classroom VR, and CrowdSign. They gave me a better idea of what already exists and what’s missing. The main thing I noticed was that most tools only cover fingerspelling and don’t really help people build sentences or learn through feedback. That helped me understand where my project could fit in.

Overall, it was a decent week of reading and taking notes. I didn’t make any major breakthroughs, but I started seeing how I could apply what I found to my own project idea.

## Week 6 - Gathering Feedback from Existing Apps
This week I decided to ask a few friends to test some of the sign language apps I found earlier. I wanted to get actual feedback from users instead of just relying on my own opinions. I used the “I Like, I Wish, What If” method to keep their responses structured and easy to compare.

The feedback from ASL Fingerspeller was mostly about the hand tracking not working properly and the lack of feedback when users made mistakes. People said it was fun and interesting at first, but frustrating when signs weren’t recognised correctly.

For CrowdSign, they liked the idea of users uploading missing ISL signs, but said it felt more like a dictionary than a proper learning tool. It was helpful for quick lookups but not great for long-term learning.

From this, I learned that if I want my Sign & Spell VR project to actually be useful, it needs to be interactive, clear, and consistent. Things like feedback and calibration need to work smoothly, or users will lose patience fast.

## Week 7 - Turning Feedback into Requirements

This week I went through all the feedback I collected and started figuring out what it means for my own project. I tried to turn their comments into actual requirements that I can use later when designing Sign & Spell VR.

For example, people wanted better calibration, clearer tutorials, and real-time feedback, so I wrote those down as things my system should include. I also added the idea of showing progress or having small goals since people liked being able to track what they’ve learned.

It wasn’t the most exciting week, but it felt good to actually make something concrete out of all the feedback. I’m still not at the stage of building anything yet, but at least now I know what users will expect from a proper ISL VR learning app.

## Week 8 - Interim Report
This week I spent most of my time working on the interim report. I had to pull everything together — the research, feedback, and early planning — and put it into the proper format. Writing it took longer than I thought because I had to make sure everything flowed logically.

I mainly worked on the introduction, project background, and literature review sections. I also added the feedback I got from ASL Fingerspeller and CrowdSign to show how it helped me figure out my user requirements.

It wasn’t the most interesting week since it was mostly writing and editing, but it did help me understand how all the pieces of my project connect. The interim report basically made me realise I’ve done a fair bit of groundwork even though I haven’t built anything yet.

## Week 9 - Interim Report 
This week I mainly focused on getting Sections 3, 4 and 5 of the interim report finished so I could stay on track with the project deadlines. I didn’t add anything very advanced, but I tried to make sure each section linked back to my Sign & Spell VR idea and showed that I had at least thought things through.  

For Section 3, I wrote about the system requirements and used the feedback from the earlier app reviews and user comments to decide what the VR app actually needs to do. I probably could have gone into more technical depth, but I at least broke things into basic modules like hand tracking, feedback, UI, and data storage so it didn’t feel completely vague.  

In Section 4, I described the system design and architecture, mostly using simple diagrams and explanations so it was clear how the different modules connect. It isn’t the most complex design ever, but it shows a straightforward flow from the user doing a sign, to the hand tracking detecting it, to the app giving feedback and saving progress.  

For Section 5, I put together my testing and evaluation plans, explaining how I’ll check if hand tracking, feedback, the interface, and data saving actually work in practice. The plan relies a lot on informal testing with friends for now, which isn’t perfect, but it at least gives me a starting point for finding bugs and improving the prototype later.

## Week 10 - Prototype Developement and Interim Report 
This week I worked on Sections 6 and 7 of the report, which meant finally putting together the actual prototype and then being honest about the problems and future work. It felt a bit rough in places, but at least I now have something running in VR instead of just plans on paper.  

For Section 6, I described what I built for the prototype: a simple Godot 4 scene using OpenXR with hand tracking set up for both hands, basic hand pose detectors, and signals that map a few ISL alphabet poses to letters in the scene. I also added basic on‑screen feedback in VR so when a pose is recognised the UI updates, plus a simple environment and addon setup to keep everything stable enough for testing.  

In Section 7, I wrote about the main issues and future work, like tracking accuracy not always being reliable, the limited number of letters supported, and the UI and feedback needing more polish. I also outlined a basic plan with tasks and a Gantt chart for improving the prototype, adding more signs, and doing better user testing later, even though the plan is still quite simple and not fully detailed.

## Over Christmas

Over the Christmas break, the plan was big: finish the full ISL alphabet A–Z, polish the VR environment, and make progress on user accounts, calibration, and data saving. In reality, holidays took over and I didn’t get to do as much as I hoped, so the project stayed at an early prototype stage. The app ran on the Meta Quest 3 in passthrough, an ISL alphabet board was visible in the scene, a feedback label showed which letter was detected, and hand tracking only worked reliably for three letters: A, V, and D.  

The focus after that was to take this small prototype and turn it into something that felt more like an actual application. The most impactful improvement was to add a main menu with user account creation, backed by JSON file saving, and then connect that smoothly to the existing VR scene. This way, instead of dropping straight into VR with no context, the experience would start with a simple flow: enter a name, create an account, and then launch into the learning environment.  

### Starting point: a basic VR prototype

The existing VR scene already contained the core pieces of Sign & Spell VR. There was an `XROrigin3D` node configured for the Meta Quest 3, with hand tracking and pose detection running through OpenXR. The ISL alphabet board floated in front of the user, acting as a visual reference for the signs. A 3D UI label in the environment displayed feedback whenever a recognised pose was detected, currently limited to the letters A, V, and D. This scene was functional but isolated: it loaded immediately when the project started, with no user, no account system, and no persistent data behind it.  

### Global script: sharing user information between scenes

To support user accounts, the first step was to create a central place to store data that multiple scenes could access, such as the active username and a consistent path for saving files. A small script called `Global.gd` was created, with a simple structure: it stores the current user’s name, and it provides a helper function that builds a per‑user save path inside Godot’s `user://` data folder, producing filenames like `Karl_calibration.json`. By loading this script as a global singleton, any scene in the project can read `Global.current_username` and use `Global.get_save_path()` to write or read that user’s data, making it much easier to manage per‑user files.  

### Building a 2D main menu scene

Even though the experience is VR, the main menu itself is just a flat 2D interface. A new scene was created using a `Control` root (the User Interface template). This scene, named `MainMenu.tscn`, is responsible for displaying the title of the app, asking the player to enter their name, and providing a button to start the experience. The layout is straightforward: a `ColorRect` fills the screen to provide a simple background, and a `VBoxContainer` in the centre stacks the UI elements—a title label (“Sign & Spell VR”), a text prompt (“Enter your name:”), a `LineEdit` for name input, and a `Button` labelled “Start / Calibrate”. This simple menu delivers a clear and familiar flow before entering VR, and it also matches the design ideas described in the interim report.  

### Implementing user account creation with JSON

The key behaviour in the menu is handled by the `MainMenu.gd` script attached to the root node. When the Start button is clicked, the script reads the text from the `LineEdit` and trims any extra spaces, checks that the name is not empty, and then stores that name in `Global.current_username` so the rest of the app can use it. It then creates a small dictionary with fields like `name` and `created_at`, writes that dictionary to a JSON file in `user://`, and uses a filename pattern such as `Karl_account.json` based on the entered name. Finally, the script switches from the menu scene to the existing VR scene (`main.tscn`). This means that each time someone enters a name, a real data file is created on disk with their account information, and the file can be inspected in the user data folder to confirm that the JSON structure is correct.  

### Wiring the menu into the application flow

To integrate the new menu into the overall application, the project’s main scene was changed to `MainMenu.tscn`. Now, when the project runs, the 2D menu appears first on the monitor (and can be mirrored into the headset). A name is typed into the text box and the Start button is pressed, a user‑specific JSON file is created and stored, and then the scene changes to the VR environment where passthrough, hand tracking, and letter detection continue as before. From the player’s perspective, the experience now starts with a clear entry point rather than dropping straight into the VR world, and it feels more like a complete application instead of a raw test scene.  

### Why this matters for the project

Even though the alphabet is still limited to A, V, and D and there wasn’t a huge amount of progress over the holidays, this focused update makes the prototype feel significantly more like a real application. User account creation is now visible and real, not just an idea described in the documentation. JSON‑based storage is implemented, laying the groundwork for saving calibration data and tracking progress later. The flow from menu to VR is seamless, matching the system architecture described earlier (menu → account → calibration → practice). The next logical steps are to connect calibration data to the same JSON file and to expand recognition from a few letters toward the full ISL alphabet, but even this single burst of work has turned a rough demo into a more structured, user‑centric prototype.
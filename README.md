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
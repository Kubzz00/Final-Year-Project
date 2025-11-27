# Final Year Project
## Sign & Spell VR: ISL Alphabet Practice and Sentence Construction in VR

**What is the Project idea?**  

My project is called Sign & Spell VR. It’s a virtual reality application that helps people learn 
Irish Sign Language (ISL) in an interactive, fun, and educational way. The idea is to let users 
go from learning ISL to spelling words, forming short sentences, and finally taking a small 
test to check what they’ve learned. It will run on the Meta Quest 3 provided in the XR 
Prototyping Module using Godot 4, and it tracks the user’s hand movements in real time to 
see if they are signing correctly. 
 
**Why is it useful/unique?**  

Most sign language learning tools focus on American Sign Language (ASL) and use videos or 
simple 2D animations. This project is different because it focuses on ISL and uses VR hand 
tracking so learning can practice in a 3D Environment. It also gives real-time feedback and 
doesn’t rely on machine learning, which keeps it fast and reliable. Later versions could add 
ML for better recognition and translation. 
 
**What does it offer (e.g., To the User)?**  

It offers users a way to practice ISL interactively instead of just watching videos. They can 
learn letters and words, combine them to make short sentences, and get feedback on how 
accurate their signs are. There’s also a test mode that checks what they remember and 
tracks their progress. 
 
**How will it Operate?**  

The app uses hand tracking from the Meta Quest 3, and the code will come from Godot 4. A 
simple rule-based compares hand positions to stored ISL sign templates. All the signs, 
words, and sentences are stored in JSON files, which makes it easier to update or expand 
later. 
 
**Why is this a good idea and what will the end deliverable be?**  

This project is a good idea because there aren’t many tools for learning ISL, especially in VR. 
It’s inclusive, educational, and uses modern technology in a useful way. The final deliverable 
will be a working VR Prototype where users can learn, practice, and test their ISL knowledge 
through interactive lessons and feedback.

## Documenting

### TODO Week 13/10/25 -> 19/10/25 
```
- Get the User Requirements from the Deaf Community 
- Check if there is a gap in the market for existing apps between ASL apps and ISL apps
-  Do a UML Case
- Write out Scope of the Project
- Plan out the Work Load
- Email Irish Deaf Society, Robert Smith (robert.smth@tudublin.ie) Irene Murtagh, John Gilligan
- Make a Consent Form (has to be anonymous)
- Make a Forms for the user testers
    - Requirements
    - What they want
    - What is Feasible to do?
- Research on FURBS
- Do weekly logs on Brightspace
```

# Weekly Logs
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
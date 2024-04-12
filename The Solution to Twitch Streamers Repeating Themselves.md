Twitch Streamers get asked the same questions over and over again.

Viewers are hyped, they react to what the Streamer does and says, and because they are so engaged with the content they are watching and connected to the person behind the screen, they ask questions in the chat. Streamers who do read the Chat and interact with their Viewers read those questions out loud and answer them, sometimes once, but most of the time every day or even multiple times a day, having the impression to repeat themselves.

The current solutions to this are:
- Pinning a message in Chat - usually done by the Broadcaster or a Moderator - so that the main information remains at the top of the Chat
- Recording dedicated videos and Live Q&A Sessions to gather all questions and answer _some_ of them
- Ignoring questions in Chat altogether

Obviously, these solutions have their pros and cons, and overall they are not as satisfying as what they could be.

While the core essence of Twitch is to offer livestreams, it comes with the FOMO (Fear of Missing Out) effect. A Follower might feel like they are missing out on something great happening when they are not watching (or listening to) the Stream. 

If during that period of time, the Streamer answered a question that the Follower did really want to know about, unless the full replay is made available online, the information, as it was officially shared, is gone forever.


Viewers,
You genuinely are interested but afraid to ask a question that maybe got answered some minutes before you joined the Stream. So you roll the dice of asking the question regardless, or you passively watch with your question in mind.

Streamers,
You try your best to answer as many questions as possible and you want to provide the best experience to your audience but end up repeating yourself or having to ignore questions you already answered.

Now, imagine a world where all the common questions you answered while Broadcasting on Twitch are made available in one centralized place.

Just streamed for 2 hours about an upcoming event you'll attend?
Viewers and you were hyped, the Hype Train went up and you were happy to pick and answer all the questions you humanly could.
You cut the Stream and _*magic*_ all those questions you answered are already categorized with tags and can be searched and filtered on one place that you made your own.

Some categories of questions are only made available to your fellow Subscribers, while some others are fully available to the public. You are in control.


This is the idea I made a reality today, with a (very) Minimum Viable Product in an afternoon.

Meet "ViewersAsk", an online platform that comes with a Twitch bot that are linked together.

I'm looking for ways to make the process of gathering questions and answers more automated with the least amount of manual steps.

For now, I created a command that can be used by Moderators (and the Streamer of course) in their Chat, to provide a question, its answer and an optional tag.

The current syntax looks like `!addq Question~Answer~Tag`.
Example: `!addq What do you think of [...]~I think it's great in the current meta because [...]~[Some game name here]`

When the command is used, the relevant information is added to a database:
- The original question
- The official answer (can be edited later)
- The category the question belongs to
- The date and time at which it was added
- The Moderator who added the command
- The unique question ID that is auto-incremented

Now all there is to do is to make a simple website that requires Twitch Authentication and a search-and-filter feature to browse all the questions.

The goal is to make a Dashboard for Streamers in which they could:
- Add and Edit questions and answers (including the category they belong to)
- Allow only specific Moderators to add questions
- Change the visibility of specific categories of questions to Sub-only, Follower-only or Public


What do you think about this tool? Let me know in the comments!
I'm open to constructive criticism and inspired to provide the best experience.
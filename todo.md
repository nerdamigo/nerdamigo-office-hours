* Stream Control Concerns:
  * Figure out rapid muting (sneezing, etc)
  * Scene switching
  * "I'm Live" notifications

* Question UX / API
  * Question data model (E: External; I: Internal)
    * E: Title (Auto extract / suggest would be fun)
    * E: Description (needs to support formatting - something like markdown)
    * E: Labels (infrastructure-as-code, security, application-design, people-process; semi-curated; can be community-sourced - but might be require moderator?)
    * I: Label Remap (allow users to submit labels dynamically, but remap to a more curated set)
    * E: Comments / Discussion (questions need to be clarified)
    * E: State (Pending Review, Pending Clarification, Ready for Answer, Being Answered, Answered)
    * E: Votes (free, but limited recharge rate) & Boosts (purchasable, but not auto-win - maybe a question can be downvoted?)
    * I: Quick Response (Rapid or automated follow up comments when a question is in need of clarification, has been deemed inadmissable, etc)
    * I: Interaction Metrics (By platform - so twitch chat, viewcount, youtube views / chat on VOD, personal site)
  * UX Views
    * Profile
    * Sign In (Cognito hosted? Or self-hosted w/ redirects)
    * Add / Edit Question
    * Current / Next Question(s) - for integration into stream

* Authentication / Authorization
  * Twitch.tv auth here makes sense (can create a twitch app)
  * Allow other federation sources? Discord / google / msft?
  * Create a cognito user store

* Community Building
  * Chat bridging (between twitch / discord)
  * OH Announcement (LinkedIn, Discord, Slack Webhook(s), Twitter)
  * Question State Changes ("Thank you" email / DM; "You're next in line"; "Please clarify"...)
  * Attendance / participation earns votes
  * Inviting people who attend earns votes

* "Question Environments"
  * Can the type of question preclude / pre-seed a sort of automated enviroment bootstrap? I.E. "The next question mentions AWS IAM, so deploy a known structure"
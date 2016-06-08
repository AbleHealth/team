
## Day in the life of an engineer at Able Health
Engineers and product work in one unified team ("product") 🌞🌚
- Every night we import data from EHRs of our customers. First thing is to quickly check if our data import pipeline is running as expected. If not, create a story and discuss during product standup. "Who could help us design a better system?" 🙋
- Mid-morning, join product standup at with product team (engineers and product manager). Review stories currently in progress, identify any blockers, help team members with any outstanding questions or issues. We coordinate who'll be running a remote 45-60m technical interview with a very promising candidate. 🙏
- Pair with another engineer on feature that's nearing completion. We review automated tests in place, write additional ones, and deploy new code to production behind feature flips. Click "deliver" and head to lunch. 💃
- Grab lunch with a couple coworkers at the Yerba Buena Gardens Festival a couple blocks away. Free music and public spaces! 💓🎵🌳 
- Back at Able, our feature looks good and was accepted! Now it's time to design a new app abstraction. We need to identify whether older patients at one of our provider clients are receiving adequate care around hypertension. First thing is to take a look at the healthcare quality measure description—thankfully, our in-house clinical measures expert did this already— and determine how to map those concepts to our domain model. After writing some tests in Ruby and forays into SQL, it looks like the work will involve updating how we import some third-party data, creating additional data models, and having that new data power visualizations in the app. 📈
- Team retro time: 
  * **Team likes**: 
    - Publicizing the team culture guide! 💌
    - A healthcare org in SF told us they love how quickly we build features that help them better coordinate patient care. 🏆
    - Shout out to the team that debugged some gnarly SQL on a measure story last week. 🙌
  * **Team wishes**: 
    - More team expertise around data integration and denormalized data. We can always use more! 🐷
  * **Team wonders**: 
    - How can we do better at sourcing potential new team members from a variety of backgrounds and experiences? 🌐
    - Who can help us build out our infrastructure on AWS using Terraform 🌏 and Docker? 🐳

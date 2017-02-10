# Able Health Hiring Assignments

The goal of the Able Health coding assignment is for you to demonstrate to us that you
have the technical skills that we need on the typical projects we do.  Most of
our current work is done in some combination of Ruby/Rails-based web work
(including Javascript and associated client side frameworks)
We want you to use this opportunity to impress us - either with some prior work
you've done or by taking on a new assignment and completing it with skill
relatively quickly.

Here's a brief comparison between junior and senior level expectations:

- *Junior Engineer* - still learning some technical skills that we
  use every day. You are still expected to to be capable of researching topics
  an applying them, but you won't be as proficient in development as people
  with more experience.
- *Senior Engineer* - not only are you a fast worker who knows their
  tools backward and forward, you also have gained wisdom through experience
  and this shows in your work.  If you're a developer, your code follows
  well-established principles (e.g. SOLID), is easy to maintain, and
  demonstrates maturity in your approach.  

Although your coding assignment should offer us some insight into where you
fall on this spectrum, it is not the only (or even primary) way we'll make
that determination.  Still, ensure that the quality of work you do as part of this
assignment is consistent with how you'd like to be viewed.

## Your Own Choice

One option you have for this assignment is to show us some work you've already
done.  While this option is fairly open-ended, please ensure:

- The work should be primarily your creation.  It's okay if you point us to
  some open source project you contributed to, but we want to evaluate your
  work, not others'.  If this is what you do, give us a commit/branch SHA on
  github or similar that isolates your work from others.
- You must be free to share the work with us. We don't want to see things for
  which you or we don't have license to see the IP.
- It should be in a language/platform that is relevant to what we do. Some contenders: Ruby/Rails, Python/Django, Go, nodejs, etc.
- It should be a substantial piece of work.  This option is designed for you to
  impress us on something that demonstrates your ability to work over a
  sustained piece of time, not a small, clever hack.  Look at some of the other
  assignments below to gain a sense of what we're hoping to get from people who
  spend a couple of days (or less) on their assignment. If you instead choose
  to submit other prior work, it should be significantly more involved than
  what you'd produce in that short amount of time.
- We should be able to build and run it. We typically look to test coverage as
  a way to help us understand the code. So, if there are special instructions
  we need to know, make sure you tell us.

If you choose to use a prior work for your coding assignment, give us a link to
github or something similar that lets us pull and evaluate it.  Please don't just zip up a source directory
and send it to us.  We need to ensure you've followed guideline 1 above.


## Something New

Your other choice is to pick up a new assignment from below.  These assignments
are designed to be completed in a few hours to a couple days. Pick one or pick
several.

### General Guidelines

- Commit often so we can see your progression.
- Open issues if you have requirements questions.
- Open pull requests if you want a code review.
- Make it easy for us to run your project locally.
- Please do not publicize these assignments.

## Assignment: Scraper Service

This assigment is an app that scrapes another site and presents the data as
a web service.

- Use Rails, Sinatra, or any other web framework that works for you.
- Pick any data-heavy site that interests you but does *not* currently have a
  public API.  (stock quotes, baseball scores, craigslist, etc.).  The more and different
  types of data you scrape and relate, the better.
- Scrape the target site on each request.
- Include documentation for how to use your web service.
- Include tests
- Deploy the service to Heroku

For extra credit, consider going above and beyond with items like:

- Cache the results for a day.
- Create a client-side app that makes use of your web service.


## Assignment: Make Twitter

This assigment is a Rails application that mimics a subset of Twitter.
Most of our code is currently in Rails, so if
you're unsure which assignment to pick, this is a good choice to show us you
know your stuff.

- Use Rails
- Use Twitter Bootstrap for styling
- Include tests
- Implement the core social network service yourself.  Don't just pick a gem
  like SocialStream.
- Base features to implement should include signup, posting new status updates,
  following other users, seeing your timeline, and favoriting tweets.
- Deploy the site to Heroku

For extra credit, consider going above and beyond with items like:

- Make your app an OAuth provider
- Create a client-side app that displays and adds posts to the timeline
- Implement several other twitter-like features (e.g. search, direct messages,
  mentions).

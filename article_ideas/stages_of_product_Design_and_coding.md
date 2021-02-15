
# Coding (4 part)

## Ideation

- General overview of what were bulding
	- What is the core use care
	- What businesses need this
	- How will someone from that business actually use it
		- User Testing if possible
- What was core to zen1, what could be trashed
	- 
- What was core but not done well, how can I do it well.
	- Reporting
	- Logging
	- Permissioning

- Register your social media/domains BEFORE you release
	- You don't want to be left out in the cold because you forgot. Please will snap up your names if they see an opportunity
		- Castlmap and zenbership.com both fell victim to this.


### Key Choices:
- All open source toolsets
	- PHP
	- Postgres
	- React
- License Selection
- Does it need multi-lingual support
- How accessible should it be


## Data Design

- Design a workable database. doesn't need to be perfect, migrations as we grow
- Get useful and complete seeding data - don't skip this step.
	- Variations in data types, etc.


## Architecture

- Clients/APIs?
	- React/Vue?
	- REST/GraphQL?
- Monolith?
- What languages and why?
	- PHP - weird choice, or is it? Businesses that used zen1 were not all cloud-savvy, need something that easily deploys to wherever other staples of php deploy, such as wordpress.
- What are core 3rd party integrations
	- Set up sandboxes with each
	- Drivers / interfaces to support multiple different providers
- Make the application extensible in a fashion that separates core code from plugin code
	- Makes updating easy without overwriting possible changes to core code.


## Don't just focus on backend - UX determines how it should be structured.

- Code shouldn't ditact how the app will be used initially, so focus on how a user will use this, both on the client side and admin dashbaord side.
	- Mock ups or crude layouts at first, don't worry about design yet.


## Start Coding

- Pick one feature that is most central to the app, and start coding it. Know that this will be imperfect and the longer you code the more it will need changes. But you have to start somewhere, so start.
- Invest of code generation once you are comfortable with the patterns you've selected.
- Limit scope of code generation to 2/3 things max. Changes will be needed, and if you can perfect those 3 use cases, 80-90% of code will be where it needs to be. So focus on this and take your time. You don't wanna be editing 10-20 resource files because a single small change may be needed.
	- Abstract anything and everything wherever you can.

## Avoiding Coding Block

- Don't be an early perfectionist. Just get the feature working, don't worry about code structure, patterns, etc. Do your best to be good about it, but if you know you're doing something that can be abstracted, belongs in a service/controller/anywhere else, isn't using consistent patterns, leave a todo note for later and address all of thoes during your once weekly code clean up day.
- Don't worry too much about testing yet - we need to establish our patterns, features, before we can handle this.
- Do: maintain your doclbocks in a way that will make generating API docs easier later.


### Be consistent with your todo labels to make finding them easier later

// TODO: language files
// TODO: interfaces
// TODO: structure
// TODO: pattern
// TODO: etc. etc. etc.


## Perfect your coding

- Within a short while, it should become clear how this will be used. Start expanding your code base, and using code generation where possible to cut time.
- Don't think too low level yet - permissions, logging, and other things that can be handled by middleware and are generally easy to implement at a later time once the full scope of the tool becomes clearer.
- If you care to, which you should, plan on writing unit tests.
	- You don't need 100% coverage, but
	- You should absolute have code coverage against core functionality
		- Core functionality is defined as anything that if it failed, would cost your customers users/money.


## Take breaks and Shift focus

- Don't get burned out doing the same thing too much.
- Throw in a design-only day once ever two weeks.
- Throw in a code-cleanup day once a week to reduce tech debt.


## Post-coding

- Security audits
- Stress testing
	- If the results aren't good enough, work on optimizing.
	- Expose the results of these in an honest way.
- Finalize and perfect the designs.
- Marketing plan execution
- Work on very well written documentation
	- I can't stress enough how important good documentation is
	- Technical + API docs for developers
	- User documentation for non-technical people
		- As a developer, very strongly consider outsourcing this to someone who can communicate in a non-technical way.
	- Consider making video tutorials.
- 


## Beta Release!

YOU ARENT EVEN CLOSE TO DONE JUST BECAUSE THE CODE IS!!! THIS IS THE MOST IMPORTANT STAGE, SO BE EXTRA CAREFUL.

- Release your software as a beta product
- Have user opt-in to data sharing and tackle what data you want to collect, exceptions, etc..
	- Be transparent and open with what you're collecting.
- Actively go get user feedback - don't wait for them to come to you
	- Bugs
	- UX issues
	- General items that are missing from existing features
- Be clear on the scope and beware of feature creep
	- Everyone is going to want something core to their business
	- You can't say yet to everything.
		- Be selective, or 
		- If you want to create a community voting system
	- Encourage open discussion via forums and BE RESPONSIVE AND HELPFUL
		- Create dedicated community forums
		- This creates an early sense of community
	- Engage on multiple platforms
		- Twitter
		- Reddit
		- Discord
		- Facebook
		- Linkedin
		- Instagram
		- etc..
- Release on a regular schedule during beta
	- Once every 2-4 weeks is a good number.
- Set a fixed beta period and plan on a release day 3-6 months after start.
- IF VC funding is in the plans, start networking and consider making introductions during this stage.
	- Don't do this before you have a usable product
	- Ideal do this once you have a captive audience
	- Anyone using this in production is ideal
- If you plan on doing a kickstarter, now is the time to start pushing it. Set a goal for well in the future and a number that can provide time for people to fall in love with the application and want to support it.


## THANK YOU COLLABORATORS, SUPPORTERS, AND BETA TESTERS

You are nothing without these people - treat them like it!

- Send hand written notes,
	- Not just once, consider doing this on holidays, etc..
- Make mentions on social media,
- If you can, provide thank you gifts.


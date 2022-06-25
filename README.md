# Grab Hackathon
### This Hackathon's objective is to help Grab honor its mission to drive Southeast Asia forward by creating economic empowerment for everyone. 
There are four themes that participant could choose for their project : 
- Creating Social Impact
- Empowering the community
- Emerging stronger
- Open format

### This repository consist the submission of my team. My roles are : 
- associate product manager : create business process of the app, think of MVP (Minimum Viable Product) that could fulfill our project's objective, propose timeline of feature improvement in the next stage, criticize the Functional Requirement, and lastly summarize all information to final proposal 
- data analyst : analyze the text data from Twitter scrapping result and summarize it as our project's background, create the Power BI dashboard to be embedded to front end of our mobile application. 

### Now We proudly present: Soombang, the integrator app for those who care!

In this app, we have 3 main components:
1. Front-end (Vue.js)
2. Back-end (Golang) -> https://bitbucket.org/jnana_parantapa/grab-hack-for-good/src/master/
3. GrabApiOrderDispatcher (Python on AWS Lambda)

To operate front-end, you can follow these instructions:
1. git clone https://github.com/farhanrbnn/grab-hackathon-nbwc
2. cd frontend
3. npm install
4. npm i -g @quasar/cli
5. quasar dev

To operate back-end, you can follow these instructions:
1. Clone repo with: `git clone https://github.com/farhanrbnn/grab-hackathon-nbwc`
2. Go to repo folder with: `cd backend`
3. Build docker with: `docker build . --tag=nbwc-team-grab-for-good-hackathon`
4. Run docker with: `docker run --publish 9090:9090 nbwc-team-grab-for-good-hackathon`

Some notes:
1. For operating the GrabApiOrderDispatcher, you can only use it via back-end, so our back-end will dispatch the order automatically on the cloud.
2. The back-end is already hosted in our cloud, so you can access it via this url: `http://ec2-52-221-244-108.ap-southeast-1.compute.amazonaws.com:9090/api/v1`.
3. We also put API docs (via JSON with Postman format) to make the reading easy.
4. Grab create delivery detail request API on {{url}}/transaction/pay/:transaction-id API on back-end won't work for local build, because it needs AWS credentials to be able queue grab create delivery detail request on AWS Lambda and AWS SQS that need 


Enjoy our app!

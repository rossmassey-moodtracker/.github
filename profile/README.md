# Moodtracker

## Description

This application will let users log their mood.

It will display metrics and predictors about their logged mood (for fun), showing how
it correlates to things such as weather.

## Repos

### [moodtracker-api](https://github.com/rossmassey-moodtracker/moodtracker-api)

Django backend
- Pulls a container from AWS ECR and runs on ECS
- Connects to a PostgreSQL database hosted on RDS
- [http://moodtracker-api-load-balanacer-129190309.us-west-1.elb.amazonaws.com/](http://moodtracker-api-load-balanacer-129190309.us-west-1.elb.amazonaws.com/)

### [moodtracker-ui](https://github.com/rossmassey-moodtracker/moodtracker-ui)

React frontend
- Static deployment to a publically accessible AWS S3 bucket
- [http://moodtracker-react-frontend-gh.s3-website-us-west-1.amazonaws.com/](http://moodtracker-react-frontend-gh.s3-website-us-west-1.amazonaws.com/)

## Tasks

### Finished
```
[X] set up basic containerized backend with token authnentication
[X] set up basic frontend
[X] deploy frontend to S3
[X] deploy backend to ECR/ECS
```
### Todo
```
[ ] hook up deployed frontend to backend
[ ] add login component to frontend
[ ] add weather access through API
[ ] seed user database with dummy data for demonstration
[ ] add data analysis and predictors for logged moods
[ ] improve UI
```


# Moodtracker

## Description

This application will let users log their mood.

It will eventually display metrics and predictors about their logged mood (for fun), showing how
it correlates to things such as weather.

## Repos

### [moodtracker-api](https://github.com/rossmassey-moodtracker/moodtracker-api)

Django backend
- Pulls a container from AWS ECR and runs on ECS
- Connects to a PostgreSQL database hosted on RDS
- **[View](http://moodtracker-api-load-balanacer-129190309.us-west-1.elb.amazonaws.com/)**

### [moodtracker-ui](https://github.com/rossmassey-moodtracker/moodtracker-ui)

React frontend
- Static deployment to a publicly accessible AWS S3 bucket
- **[View](http://moodtracker-react-frontend-gh.s3-website-us-west-1.amazonaws.com/)**

| Username | Password |
| --- | --- |
| test | moodtracker |

## Tasks

### Finished
```
[X] set up basic containerized backend with token authnentication
[X] set up basic frontend
[X] deploy frontend to S3
[X] deploy backend to ECR/ECS
[X] hook up deployed frontend to backend
[X] add login component to frontend
[X] add form to log mood
[X] add weather access through API
```
### Todo
```
[ ] add location data to mood logs
[ ] show weather info in ui
[ ] seed user database with dummy data for demonstration
[ ] add data analysis and predictors for logged moods
[ ] improve UI look
```


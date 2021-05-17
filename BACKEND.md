# Challenge - Backend Software Engineer

In this challenge you will build a simplified version of a Geofences service.
It was designed to raise doubts from your side.

## Context 

A geofence is an entity which will hold latitude and longitude informations, it also, has advertising list tied to it

In nutshell a geofences services has 3 main operations

1) Create a new geofence
2) Manage (CRUD) advertising in a geofence
3) Check for geofence entrance

## Constraints

- Create new geofence:
    - It need to consume a JSON with lat, lng and radius 
    - All values are expressed by decimal of precision 7 (max) 
    - Radius is how meters far from the center    

- Manage (CRUD) advertising in a geofence
    - It need to consume a JSON with href field 
    - Href need to be a valid URL
    - Href need to be verified (once invoked it need to return 2XX) otherwise it need to produce proper http status code

- Check for geofence entrance
    - It need to return a list of advertising regarding current lat, lng
    - It need to return empty if there's no advertising on current lat, lng
    - If there's any advertising on current lat and lng it need to return how far current lat and lng are from center of geofences

- It need to save data on database (suggested: PostgresSQL)
- It need to be hosted on git repository: Github, Gitlab or Bitbucket.
- It need to have unit tests
- It need to been wrote using Java 8
- It need to have README.md file explaning how to run

# How to deploy to Vercel

1) Create a GitHub repository and clone the "Interfact API" repository to it.
2) Once the repository is ready, go to Vercel and create a new project.
3) Import the Github repository where the cloned "Interfact API" repository is.
4) Name the project then under "Environment Variables" add:
   firebase_api_key=''
   and
   flask_secret_key=''
   Environment variables will need to be either generated or received from a team member of Interfact
5) Hit the "Deploy" button and the API will be live

# How to update the deployment

To update the deployment, push the changes to the GitHub that the Vercel deployment is linked to and the deployment will be instantly redeployed with the updates.

# Troubleshooting

- Errors can be found in the "Logs" tab of the project deployment on Vercel
- If the data being created at the endpoint seems wrong, see what is in the firebase database to see if it matches. All of the data originates from the firebase.
- The most critical part of the software that can fail is the get_intersection function in "intersectionsAPI.py" if this is edited there should be multiple checks put in place to ensure the changes did not break anything.
- To create new API endpoints, get_intersections should not be editted. 
